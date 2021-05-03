
#
1.  What’s the difference between PUT and PATCH? [Referencing](https://rapidapi.com/)
    * PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely
    * Unlike PUT, PATCH applies a partial update to the resource.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server?[Referencing](nordicapis)
    * [Nock](https://github.com/nock/nock)
    * [MockServer](https://www.mock-server.com/)
    * [mockoon](https://mockoon.com/)

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call? [Referencing](nordicapis)
* **Swagger**: 200:ok / 400: Bad request/401: Authorization missing or invalid / 404: not found	/ 5XX: Unexpected error
* **APIDocs.js** 200:ok / 400: Bad request/ 404: not found	/403: forbidden	/500: server error	
	
4. Compare and contrast SOAP and ReST? [Referencing](raygun)
    * SOAP and REST are two API styles that approach the question of data transmission from a different point of view
    * REST was created to address the problems of SOAP.


# Continuous Integration(CI) Continuous Delivery(CD)
* due to team project the overlap occure becaues 
* the server will automatically build and test the code ; to prevent build and test information for every commit on every branch CI paves what call it **Continuous Delivery(CD)** ; it's releted to Continuous deployment 

* CI : workflow strategy, development features with modular code in more manageable increments 

* CD :  developing software , that you could release it at any time , it's an extention of Continuous Delivery(CD) actually it's process that allow you to deploy 

**How GitHub fits this process**
1. webhooks : send msg to external systems about activity in your project , for each event type you can specify the subscribers who should recived a msg about the event 
    * in this case we can subscribe our CI server to recive a msg any time  someone push code to a branch
    * CI server parse the msg from GH ==> grab the current copy of projet ==> build branch ==> run the test ==> after finish it's send msg to GH status API(containing status information about the commit )==> GH use that msg to display information about commit and can even link back to more detailed information on CI server to give clearer idea of wich chanches can be integrated 
2. in conjuction with webhooks you van use deployment API 
    * to automatically notify third party system, which can retrieve a copy of the code from GH 
    * deploy the version you request to the ENV  you specify 

 # npm (node package manager)

 ## npm consists of three distinct components:

1. the website
2. the Command Line Interface (CLI)
3. the registry

## Use npm to 
1. Run packages without downloading using ``npx``.
2. Download standalone tools you can use right away.
3. Adapt packages of code for your apps, or incorporate packages as they are.
4. Share code with any npm user, anywhere.
5. Restrict code to specific developers.
6. Create organizations to coordinate package maintenance, coding, and developers.
7. Form virtual teams by using organizations.
8. Manage multiple versions of code and code dependencies.
9. Update applications easily when underlying code is updated.
10. Discover multiple ways to solve the same puzzle.
11. Find other developers who are working on similar problems and projects.

**Howto started with npm**
1. [create an account](http://www.npmjs.com/~*yourusername*)
2. use the command line interface (CLI) to install npm. 
    * ``npm install -g npm``
    * check the version ``node -v`` or ``npm -v`` 
    * Create a package.json file ``npm init``
    * Remove a package ``npm uninstall``
    * Update a package ``npm update``
    * Display npm username ``npm whoami``
    * Run a command from an npm package ``npx``


# TDD
**TDD** Test-driven development refers to a style of programming in which three activities are tightly interwoven: *coding*, *testing* and *design*


# Node HTTP 

**Node** cross-platform runtime environment that allows developers to create all kinds of server-side tools and applications in JavaScript. 

## create a simple web server using the Node HTTP package.
1. on your terminal creat a folder then ``cd file-name``
2. Using your favorite text editor for ex ``VScode``
3. Load HTTP module ``const http = require("http");``
4. declear PORT and hostname
``const hostname = "127.0.0.1";``

``const port = 8000;``
5. Create HTTP server ``const server = http.createServer((req, res) => {``

   Set the response HTTP header with HTTP status and Content type
   ``res.writeHead(200, {'Content-Type': 'text/plain'});``

    Send the response body "Hello World"
   ``res.end('Hello World\n');``

```});```

6. server starts listening
``server.listen(port, hostname, () => {``

 ``  console.log(`Server running at http://${hostname}:${port}/`);``

``})``

7. back to terminal ``node hello.js``

# Introducing Express
**Express** is the most popular Node web frameworkand is the underlying library for a number of other popular Node web frameworks

## why we use exoress :
1. Write handlers for requests with different HTTP verbs at different URL paths (routes).
2. Integrate with "view" rendering engines in order to generate responses by inserting data into templates.
3. Set common web application settings like the port to use for connecting, and the location of templates that are used for rendering the response.
4. Add additional request processing "middleware" at any point within the request handling pipeline.

**create standard Express Hello World**
``const express = require('express');``

``const app = express();``

``const port = 3000;``

``app.get('/', (req, res) => {``

  ``res.send('Hello World!')``

``});``


``app.listen(port, () => {``

  ``console.log(`Example app listening on port ${port}!`)``

``});``

