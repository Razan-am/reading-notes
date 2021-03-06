## **Redux - Additional Topics**

### ***What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?***

- The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount) of a Higher Order Component that wraps your app.

### ***When using a thunk/async action that dispatches the actual action, which do you export from your reducer?***

- You export the actions that follow the lifecycle of a request to an external API.


-------------------------------------------------------------


## **Terms**

- **middleware**: Redux middleware provides a third-party extension point between dispatching an action, and the moment it reaches the reducer. People use Redux middleware for logging, crash reporting, talking to an asynchronous API, routing, and more.

- **thunk**: Redux Thunk is a middleware that allows you to call the action creators that return a function(thunk) which takes the store's dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished.

-----------------------------------------------

### ***Redux Toolkit (RTK)***

- The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

   - "Configuring a Redux store is too complicated"
   - "I have to add a lot of packages to get Redux to do anything useful"
   - "Redux requires too much boilerplate code"


- It includes several utility functions that simplify the most common Redux use cases, including store setup, defining reducers, immutable update logic, and even creating entire "slices" of state at once without writing any action creators or action types by hand. It also includes the most widely used Redux addons, like Redux Thunk for async logic and Reselect for writing selector functions, so that you can use them right away.

### ***Purpose***

- The Redux core library is deliberately unopinionated. It lets you decide how you want to handle everything, like store setup, what your state contains, and how you want to build your reducers.

- This is good in some cases, because it gives you flexibility, but that flexibility isn't always needed. Sometimes we just want the simplest possible way to get started, with some good default behavior out of the box. Or, maybe you're writing a larger application and finding yourself writing some similar code, and you'd like to cut down on how much of that code you have to write by hand.

### ***Why You Should Use Redux Toolkit***

- Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience. It can be added at the start of a new project, or used as part of an incremental migration in an existing project.

### ***What's included inside Redux Toolkit?***

- Redux Toolkit includes the following APIs... These APIs were created to supply logic and avoid repetition.

   1. `configureStore()`
   2. `createReducer()`
   3. `createAction()`
   4. `createSlice`
   5. `createAsyncThunk`
   6. `createEntityAdapter`

-----------------------------------------------

**References:**

@By Andy Noelker/[Correct way to pre-load component data in react+redux](https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux) 

@By Andrea Chiarelli/[Async actions in Redux with Thunk or custom middleware](https://blog.logrocket.com/managing-asynchronous-actions-in-redux-1bc7d28a00c6/)

@By redux/[What is Redux Toolkit?](https://redux.js.org/redux-toolkit/overview)