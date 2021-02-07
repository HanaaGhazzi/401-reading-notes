# Hook 

- Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components.
- A Hook is a special function that lets you “hook into” React features.
- For example, useState is a Hook that lets you add React state to function components.

## When would I use a Hook?

- If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component.

![/](https://res.cloudinary.com/practicaldev/image/fetch/s--7JKP9dwh--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/proxy/1%2AaGIXCeRQTGu41okryVyECw.png)

## Rules of Hooks
Hooks are JavaScript functions, but they impose two additional rules:

- Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
- Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks. We’ll learn about them in a moment.)

## How does it work?

by convention, we use set + state-variable to name this function useState() takes a single param, which is the initial value to assign to the state variable

## Basic Hooks:
- useState
- useEffect
- useContext