# Combine reducers in a React / Redux application

Reducers are a great concept in Redux, because they allow your react application to have specific pieces of data that all update synchronously.  All reducers run against your Redux store, and then the store triggers a change event and your entire React.js application re-renders

## Whata is Combine Reducers ? 

The ``combineReducers`` helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ``createStore``.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by ``combineReducers()`` namespaces the states of each reducer under their keys as passed to ``combineReducers()``

## How it Works ? 

It turns out that Redux lets us combine multiple reducers into one that can be passed into ``createStore`` by using a helper function named ``combineReducers``.

The way we combine reducers is simple, we create one file per reducer in the reducers directory. We also create a file called ``index.js`` inside the reducers directory.
In the index.js file we import the ``combineReducers`` function from Redux and we also import all the individual reducer files.

We then invoke ``combineReducers`` and pass to it as an argument an object that contains all the individual reducers.
``combineReducers`` will combine all the reducers passed to it into a single reducing function that can then be exported as default. 

![/](http://learnwebtutorials.com/wp-content/uploads/2018/08/combining-reducers.png)

## Rules : 

Any reducer passed to ``combineReducers`` must satisfy these rules:

- For any action that is not recognized, it must return the ``state`` given to it as the first argument.

- It must never return undefined. It is too easy to do this by mistake via an early ``return`` statement, so ``combineReducers`` throws if you do that instead of letting the error manifest itself somewhere else.

- If the ``state`` given to it is ``undefined``, it must ``return`` the initial state for this specific reducer. 

> According to the previous rule, the initial state must not be ``undefined`` either. It is handy to specify it with ES6 optional arguments syntax, but you can also explicitly check the first argument for being ``undefined``.

