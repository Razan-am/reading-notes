## **Component Lifecycle / useEffect()**

### ***Why do we not need more .html pages in a multi-page React app?***

- Because `React app` consists of a single `HTML file index.html`. The views are coded in JSX format as components.And when we need to build multi-page websites in `React` we use multiple routes instead of multiple pages to handle multiple views.

### ***If we wanted a component to show up on every page, where would we put it and why?***
   - Inside a `<Route />`, so we can access it 

### ***What does routing do with the components that were rendered when a new route is requested***

- Routing is the process through which the user is navigated to different pages on a website. Rendering is the process of putting those pages on the UI. Every time you request a route to a particular page, you are also rendering that page, but not every render is an outcome of a route.`So the URL bar changes and a different view is rendered on the page`

### ***What does props.children contain?***

-  can have one element, multiple elements, or none at all, its value is respectively a single child node, an array of child nodes or undefined

>This component contains an html tag that is receiving some props and then it is displaying `{props.children}`.

>Whenever this component is invoked `{props.children}` will also be displayed and this is just a reference to what is between the opening and closing tags of the component.

### ***How do `useState()` and `this.setState()` differ?***

- `setState() Class Component`
    - Using `state` in a class component requires the building of a state object. This state object is then modified by calling `this.setState("new state")`.

- `useState() Functional Component`
    - With a functional component, we can use React hooks, specifically the `useState() hook`. This simplifies the creation of a state component and the function that updates it.

-----------------------------------------------


## **Terms**

- **State Hook**:  Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

- **Mounting and Un-Mounting**:
    - `Mounting` a file system attaches that file system to a directory (mount point) and makes it available to the system. The root (/) file system is always mounted. Any other file system can be connected or disconnected from the root (/) file system.
    - These files are not permanently affected by the mounting process, and they become available again when the file system is `unmounted`.


-----------------------------------------------

### ***effects hook***

- The Effect Hook lets you perform side effects in function components:

      // Similar to componentDidMount and        componentDidUpdate:
      useEffect(() => {
      // Update the document title using the browser API
      document.title = `You clicked ${count} times`;
      });

- Data fetching, setting up a subscription, and manually changing the DOM in React components are all examples of side effects. Whether or not you’re used to calling these operations “side effects” (or just “effects”), you’ve likely performed them in your components before.

>If you’re familiar with React class lifecycle methods, you can think of `useEffect` Hook as `componentDidMount, componentDidUpdate, and componentWillUnmount combined`.


-------------------------------------------------------------



**References:**

@By Gaurav Singhal/[Pros and Cons of Client-side Routing with React](https://www.pluralsight.com/guides/pros-and-cons-of-client-side-routing-with-react) 

@By learn/[React This Props Children](https://learn.co/lessons/react-this-props-children)

@By Logan Johnston/[useState() vs setState()](https://dev.to/johnstonlogan/react-hooks-barney-style-1hk7)
