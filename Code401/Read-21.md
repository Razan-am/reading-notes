## **useState() Hook**

### ***How does React differ from vanilla JS/HTML/CSS?***

- `React` breaks down the UI into smaller and reusable components that can move around data amongst each other. This breaking down of the UI is what gives React an edge over `Vanilla JS`.

### ***What is the primary difference between a function component and a class component?***

-  **Functional Components:**
     1. A `functional component` is just a plain `JavaScript` function that accepts props as an argument and returns a `React element`.
     2. There is no render method used in functional components.
     3. Also known as `Stateless` components as they simply accept data and display them in some form, that they are mainly responsible for rendering UI
      4. `React` lifecycle methods `for example, componentDidMount` cannot be used in functional components.

- **Class Components:**
     1. A `class component` requires you to extend from `React`. Component and create a render function which returns a `React element`.
     2. It must have the `render()` method returning `HTML`
     3. Also known as `Stateful` components because they implement logic and state.
     4. `React` lifecycle methods can be used inside class components `for example, componentDidMount`.

-----------------------------------------------


## **Terms**

- **Functional Components**: Functional components are some of the more common components that will come across while working in React. These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function.

- **Class Component**: This is the bread and butter of most modern web apps built in ReactJS. These components are simple classes (made up of multiple functions that add functionality to the application).

- **Children / Child Components**: is a special property of `React` components which contains any child elements defined within the component.

-----------------------------------------------

### ***making sense of hooks***

### ***What Are Hooks, Exactly?***

- `Hooks` let you use `React features` like state from a function ??? by doing a single function call. `React` provides a few built-in Hooks exposing the `building blocks` of React: `state, lifecycle, and context`.
Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own `custom Hooks`. This lets you turn complex problems into one-liners and share them across your application .

### ***Why Hooks?***

- Components and top-down data flow help us organize a large UI into small, independent, reusable pieces. However, we often can???t break complex components down any further because the logic is stateful and can???t be extracted to a function or another component. 

- These cases are very common and include `animations, form handling, connecting to external data sources`, and many other things we want to do from our components. When we try to solve these use cases with components alone, we usually end up with:
    - Huge components that are hard to refactor and test.
    - Duplicated logic between different components and lifecycle methods.
    - Complex patterns like render props and higher-order components.

>We think Hooks are our best shot at solving all of these problems. Hooks let us organize the logic inside a component into reusable isolated units.

-------------------------------------------------------------



**References:**

@By Afraz Momin/[React v/s Vanilla JS - When to use what?](https://dev.to/afrazchelsea/react-vs-vanilla-js-what-why-and-when-1jin) 

@By Deepak Agarwal/[Differences between Functional Components and Class Components in React](https://www.geeksforgeeks.org/differences-between-functional-components-and-class-components-in-react/)

@By Dan Abramov/[Making Sense of React Hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)
