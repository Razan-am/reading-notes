## **Advanced State with Reducers**

### ***How can we ensure that an effect hook runs only once?***

- If you only want to run the function given to `useEffect` after the initial render, you can give it an `empty array` as second argument.

### ***Can useState() update more than one state variable at the same time?***

- Unlike the `setState` in class components, the setState returned from `useState` doesn't merge objects with existing state, it replaces the object entirely. If you want to do a merge, you would need to read the previous state and merge it with the new values yourself.

### ***Is useState() synchronous?***

- `useState and setState both are asynchronous`.
    - They do not update the state immediately but have queues that are used to update the state object. This is done to improve the performance of the rendering of React components.


-----------------------------------------------


## **Terms**

- **State Hook**: Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

- **Component Lifecycle**: Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle.There are different lifecycle methods that React provides at different phases of a component’s life.

-----------------------------------------------

### ***Ultimate Guide to useReducer***

- `useReducer` is one of the additional Hooks that shipped with React 16.8. An alternative to the `useState Hook`, it helps you manage complex state logic in React applications. 

**How does `useReducer` work?**

- `useReducer` is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

- `useReducer` returns an array that holds the current state value and a `dispatch function`, to which you can pass an action and later invoke.

- **The dispatch method:**
  
   - The `dispatch function` accepts an object that represents the type of action we want to execute when it is called. It basically sends the `type of action` to the reducer function to perform its job, which, of course, is updating the state.

   - The `actions` that will be `dispatched` by our components should always be represented as one object with the `type and payload key`, where `type` stands as the identifier of the dispatched action and `payload` is the piece of information that this action will add to the state.


-  **There are three main building blocks in `Redux`:**

   - `A store` — an immutable object that holds the applications state data
   - `A reducer` — a function that returns some state data, triggered by an action type
   - `An action` — an object that tells the reducer how to change the state. It must contain a type property, and it can contain an optional payload property

- **useState vs. useReducer:**
   - Although `useState` is a Basic Hook for managing simple state transformation and `useReducer` is an Additional Hook for managing more complex state logic, it is worth noting that `useState` uses the `useReducer` internally. This implies that you could use `useReducer` for everything you can do with `useState`.
   - `useReducer` lets you avoid passing down callbacks through different levels of your component, instead allowing you to pass a provided dispatch function, which in turn will improve performance for components that trigger deep updates.And this does not imply that the `useState` updater function.

-------------------------------------------------------------



**References:**

@By Yangshun Tay/[Multiple calls to state updater from useState in component causes multiple re-renders](https://stackoverflow.com/questions/53574614/multiple-calls-to-state-updater-from-usestate-in-component-causes-multiple-re-re) 

@By Saransh Kataria/[Provide callback to useState hook like setState](https://www.linkedin.com/pulse/provide-callback-usestate-hook-like-setstate-saransh-kataria)

@By Ejiro Asiuwhu/[The ultimate guide to the React useReducer Hook](https://blog.logrocket.com/guide-to-react-usereducer-hook/)

