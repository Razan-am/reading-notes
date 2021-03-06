## **Context API - Behaviors**


### ***When you have multiple contexts, what component type should you use (class/function) and why?***

- Function component is more effecience and less complexity that the class component to deal with multiple contexts

### ***What are some good use cases for using the Context API for global state?***

- Like to use it to filter some specific data so to put it simply, global state is the data that is shared between all the components within a React application. When the state is changed, or let’s say a filter is added, the components re-render accordingly. 

### ***How can you best test context?***

- A good way to start testing in my opinion is to test that the different states of your component are showing as expected. Seems pretty easy. And mocking props in jest/enzyme is easy. However when you start adding Redux, Api calls and Context it becomes a different story.



-----------------------------------------------


-----------------------------------------------

### ***context api***

- Context provides a way to pass data through the component tree without having to pass props down manually at every level.

**When to Use Context**

- `Context` is designed to share data that can be considered `global` for a tree of React components, such as the current authenticated user, theme, or preferred language. 

**Before You Use Context**

- Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

- If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.


**API**

- `React.createContext`:
  - Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching `Provider` above it in the tree.The `defaultValue` argument is only used when a component does not have a matching Provider above it in the tree.

- `Context.Provider`:

      <MyContext.Provider value={/* some value */}>

  - Every `Context object` comes with a `Provider` React component that allows consuming components to subscribe to context changes.The `Provider component `accepts a `value prop` to be passed to consuming components that are descendants of this Provider.

- `Class.contextType`:

  - The `contextType property` on a class can be assigned a `Context object` created by React.`createContext()`. Using this property lets you consume the nearest current `value` of that Context type using `this.context`. You can reference this in any of the lifecycle methods including the render function.

        class MyClass extends React.Component {
        componentDidMount() {
            let value = this.context;
            /* perform a side-effect at mount using the value of MyContext */
        }
        componentDidUpdate() {
            let value = this.context;
            /* ... */
        }
        componentWillUnmount() {
            let value = this.context;
            /* ... */
        }
        render() {
            let value = this.context;
            /* render something based on the value of MyContext */
        }
        }
        MyClass.contextType = MyContext;

- `Context.Consumer`:

  - A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

        <MyContext.Consumer>
        {value => /* render something based on the context value */}
        </MyContext.Consumer>

- `Context.displayName`:

  - Context object accepts a displayName string property. React DevTools uses this string to determine what to display for the context.

        const MyContext = React.createContext(/* some value */);
        MyContext.displayName = 'MyDisplayName';

        <MyContext.Provider> // "MyDisplayName.Provider" in DevTools
        <MyContext.Consumer> // "MyDisplayName.Consumer" in DevTools


-------------------------------------------------------------


## **Terms**

- **context**: React Context is a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree.

- **useContext()**: “useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.

- **static context**: a collection of methods that stand up a static store which can be accessed via HOC or plain object reference. In this way the store is reduced to a basic state/setState api which is familiar to react developers.

-----------------------------------------------

**References:**

@By Malin Milford/[https://itnext.io/jest-tests-with-react-context-api-90f3d2e06c8f](https://itnext.io/jest-tests-with-react-context-api-90f3d2e06c8f) 

@By reactjs/[Context](https://reactjs.org/docs/context.html)
