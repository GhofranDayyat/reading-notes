# Express Routing 
**Routing** refers to how an application’s endpoints (URIs) respond to client requests.

## Routing Types
1. Route methods: as GET method route POST method route
2. Route paths :in combination with a request method, define the endpoints at which requests can be made.
3. Route parameters:  are named URL segments that are used to capture the values specified at their position in the URL. 
4. Route handlers: You can provide multiple callback functions that behave like middleware to handle a request. 
5. Response methods:The methods on the response object (res) 
6. app.route() :used to create chainable route handlers for a route path Because the path is specified at a single location, creating modular routes is helpful, as is reducing redundancy and typos
7. express.Router: class to create modular, mountable route handlers.



# Express Router

**Express Router**: It is a mini express application without an express application, just the routing stuff. 
``var router = express.Router();``
1. Basic Routes: Home, About

``router.get('/',CB)``
2. Route Middleware to log requests to the console

``router.use(function(req, res, next) {}``
3. Route with Parameters
``router.get('/hello/:name',CB)``
4. Route Middleware for Parameters to validate specific parameters
``router.param('name', function(req, res, next, name) {}``
5. Login routes  define multiple actions on a single login route. We'll need a *GET* route to show the login form and a *POST* route to process the login form.
``app.route('/login')``
``.get(function(req, res) {}``
``.post(function(req, res) {}``

6. Validates a parameter passed to a certain route

# ES6 Classes

