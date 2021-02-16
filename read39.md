# Redux Toolkit

## What is redux toolkit? 
Redux Toolkit is our official, opinionated, batteries-included toolset for efficient Redux development. ... It also includes the most widely used Redux addons, like Redux Thunk for async logic and Reselect for writing selector functions, so that you can use them right away. 


Redux Toolkit is beneficial to all Redux users regardless of skill level. It can be added as an internal part of the project at the start or can be added during the internal up-gradation in the existing one 

## What is Redux used for? 
Redux is used mostly for application state management. To summarize it, Redux maintains the state of an entire application in a single immutable state tree (object), which can't be changed directly. When something changes, a new object is created (using actions and reducers)


## How Use it ? 


1. Create a "store" with "configureStore"

A store holds all your data and the actions that change that data

Use a "Provider" component (like context) to give the store to all your components

Provider gives the store to any component below it in the app. configureStore can also configure middleware and enhancers

All your data and actions to update that data. Divided into slices. All components under the Provider have access to any data or actions in the store

2. Create named "slices"

A slice holds a chunk of the state, plus the functions that can update that state

No more changing 4 different files just to write one action! 🎉

Each slice has a name. State can contain any serializable data that you want (strings, objects, arrays, etc). Reducers auto-create actions No need for 4 different files  just for 1 action!

3. Add the slice to your store by adding the "reducer" from the slice to the "reducer" in the store

The slice ".reducer" (singular) is auto-created when you define your "reducers:" (plural) in the slice

Specify the reducer name (same as your slice name). Add multiple slices by adding multiple keys to the object. Each slice has a "reducer" (singular) that is exported automatically

4. Functions that update the state in your slice are "reducers"

A reducer takes the current state and the action (data) being performed,

and updates the data in the slice's state

(redux-toolkit uses immer, so those state changes are actually non-mutating)

Reducers are functions that take the current state and change it. This LOOKS like a mutating change but since redux-toolkit uses immer, it’s actually a non-mutating change. Functions in this reducers object are auto-exported as "actions" that can be used later

5. To get values from the store in a component, use a "selector"

A selector function is given the entire redux store and returns just the data you want

Pass your selector to the "useSelector" hook which will call it for you

You can use useSelector in any component in the tree under a Provider component. The entire redux store. Access your named slice. Get any value from that slice. Then use that value like any other value in JSX

6. To change data in the store, use the "actions" that are exported from the slice

These actions are named based on your named reducers

You don't call on their own however, because they need the current state and action params

actions are created based on your reducers in your slice. actions are functions, but don’t call them directly - they have to be dispatched

7. To call the action, you "dispatch" it to the store

Use the "useDispatch" hook to get access to the "dispatch" function

then dispatch your action using that function

this automatically updates all components using "useSelector"

useDispatch can be used in any component under the Provider. dispatch is a function that takes the result of calling your actions. Make sure to call your action functions!. Then onClick, this will dispatch the "down" action to the store

A counter counting up

8. Actions can take params as well, which are passed in as the second argument to the reducer

the action "payload" will contain whatever is passed to the action

(to pass multiple params, use an object)

The dispatched action comes across as the second argument to the reducer functions. The action payload contains the params passed to the  action function

Your actions can now take params and pass those values to the reducers as the "payload"

A counter going up and down by ones and fives

9. For async actions (like fetching data), you can use redux-thunk (already included!)

Create a thunk (function that returns a function)

it's async and gets dispatch as a param

dispatch inside your thunk function

Then dispatch that action like normal in component

A thunk is a function that returns a function. The returned function will get immediately called and given dispatch as a param. Perform async actions like data fetching. Then dispatch whenever your data is ready

Your thunk can then be dispatched like any other action!

Counter counting up by 1, and then counting up by the length of text returned by localhost

10. What about just using Context instead?

Yes, I generally start projects with just context, but redux can have some advantages for larger projects or teams:

provides structure that context doesn't
can be easier to test
redux dev tools are pretty cool 