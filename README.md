# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js servers where long-running requests can cause the server to hang and become unresponsive. The `server.js` file contains a simple HTTP server with a simulated long-running task.  This task blocks the event loop, preventing the server from handling other requests.

The solution, in `serverSolution.js`, demonstrates using asynchronous operations or worker threads to prevent the main event loop from being blocked.  This ensures the server remains responsive even during lengthy operations. 