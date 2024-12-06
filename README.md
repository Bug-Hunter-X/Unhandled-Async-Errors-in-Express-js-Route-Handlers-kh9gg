# Unhandled Asynchronous Errors in Express.js

This repository demonstrates a common error in Express.js applications: unhandled errors within asynchronous route handlers.  When an asynchronous operation (like a database query or external API call) fails, the application might crash silently without providing any indication of the error. This makes debugging and maintaining the application challenging.

The `bug.js` file shows an Express.js server with a route handler that performs an asynchronous operation.  The operation is intentionally designed to fail.  Crucially, error handling is missing, leading to a silent crash. 

The `bugSolution.js` file provides a corrected version with proper error handling. It demonstrates how to catch and gracefully handle errors within asynchronous handlers, improving the application's resilience and making debugging easier.