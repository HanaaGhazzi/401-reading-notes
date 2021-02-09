# Context API


_It is provides a means of passing state down the component tree through a Provider/Consumer relationship, is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. Also we can avoid passing props through intermediate elements._

![/](https://miro.medium.com/max/3472/1*Jx8BCxZFN2SCuhQtZqfgMQ.jpeg)

## Before Use Context

- Context is primarily used when some data needs to be accessible by many components at different nesting levels.
- Apply it sparingly because it makes component reuse more difficult.


### React.createContext
When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

### Why Do We Need The Context API?

We want to build a “theme toggler” component which toggles between light mode and dark mode for our React app. Every component has to have access to the current theme mode so they can be styled accordingly.

> Context provides a way to pass data through the component tree without having to pass props down manually at every level.”