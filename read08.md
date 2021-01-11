# Express Routing & Connected API

## Express Routing:
- routing changes the roles of the files in the server, the index.js is the Entry point, server.js is the exported server, models are for data and are known as data models, routes are for the routes and handlers.

- Routes can be managed in separate modules from the main server, Routing refers to how an application’s endpoints (URIs) respond to client requests.

- For example, app.get() to handle GET requests and app.post to handle POST requests.

## what is Express API?
- The way to construct a web API is to follow the RESTful approach . REST APIs are resource-based interfaces. On the web this means that data resources are represented by URIs (paths) accessed via HTTP.

- Express 4.0 comes with the new Router. Router is like a mini express application. It doesn't bring in views or settings, but provides us with the routing APIs like .use, .get, .param, and route.

## Express Middleware
- Express Middleware A series of functions that the request “goes through” Each function receives request, response and next as parameters

- Route Middleware router.use() Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.
