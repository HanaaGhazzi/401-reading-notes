# Props and State


## setState :

- ``setState()`` is the only legitimate way to update state after the initial state setup. Let’s say we have a search component and want to display the search term a user submits.

- Update to a component state should be done using ``setState()``

- You can pass an object or a function to ``setState()``

- Pass a function when you can to update state multiple times

- Do not depend on this.state immediately after calling ``setState()`` and make use of the updater function instead. 


## Handling Events:

- React events are named using camelCase, rather than lowercase.

- With JSX you pass a function as the event handler, rather than a string.

- you cannot return false to prevent default behavior in React. You must call preventDefault explicitly.


## Components and Props

- Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. 

- Always start component names with a capital letter.

- React treats components starting with lowercase letters as DOM tags. For example, ``<div />`` represents an HTML div tag, but ``<Welcome /> `` represents a component and requires Welcome to be in scope.

## The Virtual DOM

- A virtual DOM object is a representation of a DOM object, like a lightweight copy. 

-  Manipulating the virtual DOM is much faster, because nothing gets drawn onscreen. Think of manipulating the virtual DOM as editing a blueprint, as opposed to moving rooms in an actual house.

**what happens when you try to update the DOM in React:**

- The entire virtual DOM gets updated.
- The virtual DOM gets compared to what it looked like before you updated it. React figures out which objects have changed.
- The changed objects, and the changed objects only, get updated on the real DOM.
- Changes on the real DOM cause the screen to change.


