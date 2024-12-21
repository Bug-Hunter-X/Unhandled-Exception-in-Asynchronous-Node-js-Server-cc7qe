# Unhandled Exception in Asynchronous Node.js Server

This repository demonstrates a common error in Node.js applications: unhandled exceptions within asynchronous operations.  The `bug.js` file contains a server that simulates an asynchronous task.  Sometimes, this task fails, throwing an exception that isn't caught, causing the server to crash.  The `bugSolution.js` file shows how to properly handle this using error handling techniques.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `node bug.js`.
4. Observe the server's behavior.  The server will crash intermittently because of the unhandled exception.

## Solution

The solution involves using a `try...catch` block within the asynchronous operation or using the `domain` module to catch exceptions across asynchronous calls. The `bugSolution.js` file shows how this is done with the try catch block.