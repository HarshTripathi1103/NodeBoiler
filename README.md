# ServerBoiler

ServerBoiler is a lightweight npm package that simplifies the process of creating an HTTP server using Node.js. It allows you to define your own port and quickly set up a basic server for your web applications.

# Installation
You can install ServerBoiler using npm:
```
npm install serverboiler
```

# Usage
Import the serverboiler function from the package:
import { serverboiler } from "serverboiler";
```
const myPort = 4000; // Set your preferred port
serverboiler(myPort);
```
# What this Does 
it simply converts this 
``` // fileName : server.js 
// Example using the http module
const http = require('http');

// Create an HTTP server
const server = http.createServer((req, res) => {
    // Set the response headers
    res.writeHead(200, { 'Content-Type': 'text/html' });

    // Write the response content
    res.write('<h1>Hello, Node.js HTTP Server!</h1>');
    res.end();
});

// Specify the port to listen on
const port = 3000;

// Start the server
server.listen(port, () => {
    console.log(`Node.js HTTP server is running on port ${port}`);
});
```
to this 👇
```
serverboiler(3000);
```


Your Node.js HTTP server will now be running on the specified port. You can customize the server logic within the serverboiler function.Hope this package helps you for your node js project.

# Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

# License
This project is licensed under the MIT License - see the LICENSE file for details.

Created by ❤️ from Mumbai.
