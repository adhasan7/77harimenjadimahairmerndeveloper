# 80 hari menjadi mahair mern developer
Tips 33 Hari Menjadi Mahir Mern Developer

Disini saya akan membuat Materi apa saja yang dibutuhkan untuk mencicil waktu kita selama 77 hari menjadi mern developer .

Hari 1 = intoduction-node.js
https://medium.com/@adsansapu/hari-1-menjadi-mern-developer-a6bb57928fc0

Hari 2 = Setup-node.js
https://medium.com/@adsansapu/setup-node-js-e94120b2e30a

Hari 3 =  1st Application

Node.js is an open source, cross-platform server environment which executes JavaScript using V8 JavaScript Engine. Node.js helps to write front-end and back-end code in the same language. It helps to write efficient code for real-time applications. In Node.js, the applications can be written using console-based method or web-based method.

Console based Node.js Application: The Node.js console-based applications are run using Node.js command prompt. Console module in Node.js provide a simple debugging console. Node.js is a global console which can be used for synchronous as well as asynchronous communication. The console.log() function is used to display output on console. This function prints output to stdout with newline.

Syntax:

console.log([data][, ...]);
Here, data is the content to be displayed on console.

Example 1: Creating a Hello World application using Node.js. Create a geeks.js file containing the following code:

console.log('Hello World');  
Run the file on Node.js command prompt using command node geeks.js i.e. node <file_name> .
Output:


Example 2: Creating a Hello World application receiving the user input. Create a gfg.js file containing the following code.

console.log(process.argv.slice(2)); 
The process.argv is used to provide command line argument to a program. Use the slice function with 2 as its argument to get all the elements of argv that comes after its second element, i.e. the arguments the user entered The first argument is location of the Node.js binary which runs the program and the second argument is location of the file being run.
Output:


Web-based Node.js Application: A web-based Node.js application consists of the following three important components:

Import required modules: Load Node.js modules using the require directive. Load http module and store returned HTTP instance into a variable.
Syntax:
var http = require("http");
Create server: Create a server to listen the client’s requests. Create server instance using createServer() method. Bind server to port 8080 using listen method associated with server instance.
Syntax:
http.createServer().listen(8080);
Read request and return response: Read the client request made using browser or console and return the response. A function with request and response parameters is used to read client request and return response.
Syntax:
http.createServer(function (request, response) {...}).listen(8080);
Example: This example create a Hello World web-based application using Node.js. Create a firstprogram.js file containing the following code.

// Require http header 
var http = require('http'); 
   
// Create server 
http.createServer(function (req, res) { 
  
    // HTTP Status: 200 : OK 
    // Content Type: text/html 
    res.writeHead(200, {'Content-Type': 'text/html'}); 
      
    // Send the response body as "Hello World!"   
    res.end('Hello World!'); 
  
}).listen(8080); 
Run the file on Node.js command prompt using command node firstprogram.js and type http://127.0.0.1:8080/ in a web browser to see the output.
Output:




Whether you're preparing for your first job interview or aiming to upskill in this ever-evolving tech landscape, GeeksforGeeks Courses are your key to success. We provide top-quality content at affordable prices, all geared towards accelerating your growth in a time-bound manner. Join the millions we've already empowered, and we're here to do the same for you.
