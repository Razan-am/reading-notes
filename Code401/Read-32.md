## **Redux - Combined Reducers**

### ***How granular should your reducers be?***

- A Redux app really only has one reducer function: the "root reducer" function that you will pass to createStore later on. That one root reducer function is responsible for handling all of the actions that are dispatched, and calculating what the entire new state result should be every time.

### ***Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched***
 
- Pro, Since the state of a complex app could be really wide, there is not a single reducer, but many reducers for any kind of action.

### ***Name a strategy for preventing the above***

- Make a reducer for each component that will be affected by the dispatcher, only effecting a specific amount of the state it self.


-------------------------------------------------------------


## **Terms**

- **store**: A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer. 

- **combined reducers**: it is simply a utility function to simplify the most common use case when writing Redux reducers.


-----------------------------------------------

### ***Understanding Asynchronous Redux Actions with Redux Thunk***

- By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

- There are two very popular middleware libraries that allow for side effects and asynchronous actions: `Redux Thunk and Redux Saga`.

### ***Redux Thunk***

- Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

- The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.

- It is useful when utilizing a Redux store and relying upon external APIs.
