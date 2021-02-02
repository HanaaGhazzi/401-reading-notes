# Routing !

> React Router keeps your UI in sync with the URL. It has a simple API with powerful features like lazy code loading, dynamic route matching, and location transition handling built right in. Make the URL your first thought, not an after-thought.

**useHistory** 

The useHistory hook gives you access to the history instance that you may use to navigate.

**useLocation** 

The useLocation hook returns the location object that represents the current URL. You can think about it like a useState that returns a new location whenever the URL changes.This could be really useful e.g. in a situation where you would like to trigger a new “page view” event using your web analytics tool whenever

**useParams**
useParams returns an object of key/value pairs of URL parameters. Use it to access match.params of the current ``<Route>``.

![/](https://s1.o7planning.com/en/12137/images/26763049.png)

### What does the ``<Route>`` render?

Routes have three props that can be used to define what should be rendered when the route’s path matches. Only one should be provided to a ``<Route>`` element.

- __component__ — A React component. When a route with a component prop matches, the route will return a new element whose type is the provided React component (created using React.createElement).
- __render__ — A function that returns a React element 5. It will be called when the path matches. This is similar to component, but is useful for inline rendering and passing extra props to the element.
- __children__ — A function that returns a React element. Unlike the prior two props, this will always be rendered, regardless of whether the route’s path matches the current location.

