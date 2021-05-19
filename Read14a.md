# **CSS Transforms, Transitions, and Animations**


## ***Transforms***
- by the `transform property`,now we can  can be revisited with alternative ways to size, position, and change elements. 
- It's take two different settings, `two-dimensional` and `three-dimensional`.

### **Transform Syntax**
- It's including the `transform property` followed by the `value`. The value specifies the transform type followed by a specific amount inside parentheses.

>Example:

`div {`

   `transform: scale(1.5);`

`}`

### **2D Transforms**
- **2D Rotate**
  - `rotate value` provides the ability to rotate an element from`0 to 360` degrees.

>Example:

`.box-1 {`

  `transform: rotate(20deg);`

`}`

`.box-2 {`

  `transform: rotate(-55deg);`

`}`

- **2D Scale**
  -  `scale value` allows you to change the appeared size of an element.

>Example:

`.box-1 {`
  `transform: scale(.75);`

`}`

`.box-2 {`

  transform: scale(1.25);`

`}`

>It can also write for each axis as :
`.box-1 {transform: scaleX(.5);}`//
`.box-2 {transform: scaleY(1.15);}`//
`.box-3 {transform: scale(.5, 1.15);}`

- **2D Translate**
  - `translate value` works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document,by using the `translateX value` and the `translateY value`.

>Example:

`box-1 {`

  `transform: translateX(-10px);`

`}`

`.box-2 {`

  `transform: translateY(25%);`

`}`

`.box-3 {`

  `transform: translate(-10px, 25%);`

`}`

- **2D Skew**
  - `skew`, is used to distort elements on the `horizontal axis, vertical axis, or both`.

>Example:

`.box-1 {`

 `transform: skewX(5deg);`

`}`

`.box-2 {`

  `transform: skewY(-20deg);`

`}`

`.box-3 {`

  `transform: skew(5deg, -20deg);`

`}`

- **Combining Transforms**
  - it's multipling transforms to be used at once, rotating and scaling the size of an element at the same time for example. 

>Example:

`.box-1 {`

  `transform: rotate(25deg) scale(.75);`

`}`

`.box-2 {`

  `transform: skew(10deg, 20deg) translateX(20px);`

`}`

- **Transform Origin**
  - `transform-origin property` may be used to change this default origin positionfor the default transform origin that is the centeralized of an element, both 50% horizontally and 50% vertically. 

>Example:

`box-1 {`

  `transform: rotate(15deg);`

  `transform-origin: 0 0;`

`}`

`.box-2 {`

  `transform: scale(.5);`

  `transform-origin: 100% 100%;`

`}`

`.box-3 {`

  `transform: skewX(20deg);`

  `transform-origin: top left;`

`}`

`.box-4 {`

  `transform: scale(.75) translate(-10px, -10px);`

  `transform-origin: 20px 50px;`

`}`

- **Perspective**
  -  `perspective` it's like a vanishing point, similar to that which can be seen in three-dimensional drawings.

>Example:

`.box {`

  `transform: perspective(200px) rotateX(45deg);`

`}`

## ***Transitions***

- It's an element must have a change in state, and different styles must be identified for each state.,it's determining styles for different states by using the `:hover, :focus, :active, and :target pseudo-classes`.

>Example:

`.box {`

  `background: #2db34a;`

  `transition-property: background;`

  `transition-duration: 1s;`

  `transition-timing-function: linear;`

`}`

`.box:hover {`

  `background: #ff7b29;`

`}`

- **Transitional Property**
  - `transition-property`it's determines exactly what properties will be altered in conjunction with the other transitional properties. 

>Example:

`transition-property: background, border-radius;`

>the more popular transitional properties include the following:
   ```<background-color,background-position,border-color,border-width,border-spacing,bottom,clip,color,crop,font-size,font-weight,height,left,letter-spacing,line-height,margin,max-height,max-width,min-height,min-width,opacity,outline-coloro,utline-offset,outline-width,padding,right,text-indent,text-shadow,top,vertical-align,visibility,width,word-spacing,z-index.>```

- **Transition Duration**
  - The duration in which a transition takes place is set using the `transition-duration property`.

>Example:

  `transition-duration: .2s, 1s;`

- **Transition Timing**
  - `transition-timing-function property` is used to set the speed in which a transition will move.

>Example:

  `transition-timing-function: linear, ease-in;`

>A few of the more popular keyword values for the transition-timing-function property:
   - `linear, ease-in, ease-out, and ease-in-out`.

- **Transition Delay**
  -  `transition-delay property` to determines how long a transition should be stalled before executing. 

>Example:

`.box {`

  `background: #2db34a;`

  `border-radius: 6px`

  `transition-property: background, border-radius;`

  `transition-duration: .2s, 1s;`

  `transition-timing-function: linear, ease-in;`

  `transition-delay: 0s, 1s;`

`}`

`.box:hover {`

  `background: #ff7b29;`

  `border-radius: 50%;`

`}`

- **Shorthand Transitions**
  - `shorthand property` by using `transition`, is capable of supporting allthe previous properties and values.

>Example:

`.box {`

  `background: #2db34a;`

  `border-radius: 6px;`

  `transition: background .2s linear, border-radius 1s ease-in 1s;`

`}`

`.box:hover {`

  `color: #ff7b29;`

  `border-radius: 50%;`

`}`


## ***Animations***

- **`Animations Keyframes`**
- The `@keyframes rule` includes the animation name, any animation breakpoints, and the properties intended to be animated.

>Example:

`@keyframes slide {`

  `0% {`

   `left: 0;`

   `top: 0;`

  `}`

  `50% {`

   `left: 244px;`

   `top: 100px;`

  `}`

  `100% {`

   `left: 488px;`

   `top: 0;`

  `}`

`}`

- **Animation Name**
  - `animation-name property` is used with the animation name, identified from the `@keyframes rule`, as the property `value`.

>it's applied to the element in which the animation is to be applied to. 

>Example:

`.stage:hover .ball {`

 `animation-name: slide;`

`}`

- **Animation Duration, Timing Function, & Delay**
  - to start, animations need a duration declared using the `animation-duration property`. 

>Example:

`.stage:hover .ball {`

  `animation-name: slide;`

  `animation-duration: 2s;`

  `animation-timing-function: ease-in-out;`

  `animation-delay: .5s;`

`}`


- **Animation Iteration**
  -  `animation-iteration-count property`  used to have an animation repeat itself numerous times.

>Using an `integer` will repeat the animation as many times as specified, while the `infinite` keyword will repeat the animation indefinitely in a never ending fashion.

>Example:

`.stage:hover .ball {`

  `animation-name: slide;`

  `animation-duration: 2s;`

  `animation-timing-function: ease-in-out;`

  `animation-delay: .5s;`

  `animation-iteration-count: infinite;`

`}`

- **Animation Direction**
  - `animation-direction property` used when you want to set the number of times to an animation repeats.

> Values for the `animation-direction property` include `normal, reverse, alternate, and alternate-reverse`.

>Example:

`.stage:hover .ball {`

  `animation-name: slide;`

  `animation-duration: 2s;`

  `animation-timing-function: ease-in-out;`

  `animation-delay: .5s;`

  `animation-iteration-count: infinite;`

  `animation-direction: alternate;`

`}`

- **Animation Play State**
 - `animation-play-state property` allows an animation to be `played or paused` using the `running and paused` keyword values respectively.

>Example:

`.stage:active .ball {`

  `animation-play-state: paused;`

`}`

- **Animation Fill Mode**
   - `animation-fill-mode property` identifies how an element should be styled either before, after, or before and after an animation is run.

>The `animation-fill-mode property` accepts four keyword values, including `none, forwards, backwards, and both`. 

>Example:

`.stage:hover .ball {`

  `animation-name: slide;`

  `animation-duration: 2s;`

  `animation-timing-function: ease-in-out;`

  `animation-delay: .5s;`

  `animation-fill-mode: forwards;`

`}`

- **Shorthand Animations**
  - It can be written out in a shorthand format with one `animation property`.

>Example:

`.stage:hover .ball {`

  `animation: slide 2s ease-in-out .5s infinite alternate;`

`}`


**References:**

@Shay Howe /[Transforms, Transitions, and Animations
](https://learn.shayhowe.com/advanced-html-css/css-transforms/)


