 # Redux - Asynchronous Actions

 ``Thunk`` is a programming concept where a function is used to delay the evaluation/calculation of an operation.

Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

Redux reducers must never contain **"side effects"**. A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like:

- Logging a value to the console
- Saving a file
- Setting an async timer
- Making an AJAX HTTP request
- Modifying some state that exists outside of a function, or mutating arguments to a function
- Generating random numbers or unique random IDs (such as Math.random() or Date.now())

>   "async function middleware" let us pass a function to dispatch! Inside that function, we were able to write some async logic (an HTTP request), then dispatch a normal action object when the request completed.

----------------

Just like with a normal action, we first need to handle a user event in the application, such as a click on a button. Then, we call dispatch(), and pass in something, whether it be a plain action object, a function, or some other value that a middleware can look for.

Once that dispatched value reaches a middleware, it can make an async call, and then dispatch a real action object when the async call completes.


![/](https://redux.js.org/assets/images/ReduxAsyncDataFlowDiagram-d97ff38a0f4da0f327163170ccc13e80.gif)



- **Redux middleware were designed to enable writing logic that has side effects**

- "Side effects" are code that changes state/behavior outside a function, like AJAX calls, modifying function arguments, or generating random values

- **Middleware add an extra step to the standard Redux data flow**

- Middleware can intercept other values passed to dispatch
- Middleware have access to dispatch and getState, so they can dispatch more actions as part of async logic

- **The Redux "Thunk" middleware lets us pass functions to dispatch**

- "Thunk" functions let us write async logic ahead of time, without knowing what Redux store is being used
- A Redux thunk function receives dispatch and getState as arguments, and can dispatch actions like "this data was received from an API response"