# Express

## What is Express Middleware?
**Middleware literally means anything you put in the middle of one layer of the software and another. Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it’s attached to. In fact, Express itself is compromised wholly of middleware functions. Additionally, middleware can either terminate the HTTP request or pass it on to another middleware function using next (more on that soon). This “chaining” of middleware allows you to compartmentalize your code and create reusable middleware.**

## Third-Party Express Middleware
You’ve built a couple of custom middlewares to far, but there are lots of packages already built to do the things you might normally want to do. In fact, you’ve used the simple routing middleware library by using the app.get() or app.post() middleware functions. There are thousands of middleware libraries for doing things like parsing incoming data, routing, and authorization.

## Order of Middleware Calls
One of the most important things about middleware in Express is the order in which they are written/included in your file; the order in which they are executed, given that the route matches also needs to be considered. For example, in the following code snippet, the first function executes first, then the route handler and then the end function. This example summarizes how to use middleware before and after route handler; also how a route handler can be used as a middleware itself.

## Supertest:
The motivation with this module is to provide a high-level abstraction for testing HTTP, while still allowing you to drop down to the lower-level API provided by superagent.

![/](https://miro.medium.com/max/1042/1*uwNmNlj_t6NSVLULu3R5ug.png)
