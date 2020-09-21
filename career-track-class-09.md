Express Routing
  1. Routing refers to how an application’s endpoints (URIs) respond to client requests.
  2. A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.
  3. Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.
  4. Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.
  5. Route handlers can be in the form of a function, an array of functions, or combinations of both.
  6. Response Methods - The methods on the response object (res) in the following table can send a response to the client, and terminate the request-response cycle. If none of these methods are called from a route handler, the client request will be left hanging.
    6.a.res.download() - Prompt a file to be downloaded.
    6.b. res.end()	End the response process.
    6.c. res.json()	Send a JSON response.
    6.d. res.jsonp()	Send a JSON response with JSONP support.
    6.e. res.redirect()	Redirect a request.
    6.f. res.render()	Render a view template.
    6.g. res.send()	Send a response of various types.
    6.h. res.sendFile()	Send a file as an octet stream.
    6.i. res.sendStatus()	Set the response status code and send its string representation as the response body.
  7. You can create chainable route handlers for a route path by using app.route(). Because the path is specified at a single location, creating modular routes is helpful, as is reducing redundancy and typos.
  8. Use the express.Router class to create modular, mountable route handlers. A Router instance is a complete middleware and routing system; for this reason, it is often referred to as a “mini-app”.
  
SuperTest
  1. npm install supertest || Once installed it can now be referenced by simply calling require('supertest');
  
Express Middleware
  1. Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.
  2. Middleware functions can perform the following tasks:
    2.a. Execute any code.
    2.b. Make changes to the request and the response objects.
    2.c. End the request-response cycle.
    2.d. Call the next middleware function in the stack.
  3. Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. These functions are used to modify req and res objects for tasks like parsing request bodies, adding response headers, etc.

