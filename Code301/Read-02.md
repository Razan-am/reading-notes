## **React lifecycle**

### ***Based off the diagram, what happens first, the `render` or the `componentDidMount`?***


- The `render` comes first when an instance of a component is being created and inserted into the DOM it occurs during the mounting phase.

### ***What is the very first thing to happen in the lifecycle of React?***

- In the lifecycle of React the first thing that happened is the **Mounting**,which includes these methods that are called in the following order when an instance of a component is being created and inserted into the DOM:

   - constructor()
   - static getDerivedStateFromProps()
    - render()
    - componentDidMount().

### ***Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`:***

- The order for the previous methods is:
   - constructor
   - render
   - componentDidMount
   - React Updates
   - componentWillUnmount
 

### ***What does componentDidMount do?***

- `componentDidMount()` is a hook that gets invoked right after a React component has been mounted aka after the first `render()` lifecycle.

---------------------------------------------------

## **React State Vs Props**

### ***What types of things can you pass in the props?***

- Props `(aka properties)` in React allows us to pass values from a `parent component` down to a `child component`. The values can be any data type, `from strings to functions, objects, etc`.

### ***What is the big difference between props and state?***

- The `props` allows you to pass into the componants. But the `state` is handeled inside that componant which is `props` are handeled outside it.
- The `state` it can be apdate it inside it's componant , while the `props` it's need to be apdate it outside because it's located outside the componant.

### ***When do we re-render our application?***

- The re-rendere happened when we change the `state` inside the application.A simple update of the `state`, from anywhere in the code, causes all the User Interface (UI) elements to be re-rendered automatically.

### ***What are some examples of things that we could store in state?***

- Like a counter application 
- Inside the forms

------------------------------------------------------------------------------------------------------


**References:**

@Joshua Blankenship/[React: Component Lifecycle Events](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)


@Web Dev Simplified/[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)