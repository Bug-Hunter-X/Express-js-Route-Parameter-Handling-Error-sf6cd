# Express.js Route Parameter Handling Error

This repository demonstrates a common error in Express.js route parameter handling:  incorrect error handling when a user is not found.

## Bug
The `bug.js` file contains the buggy code.  When a user ID is not found, it does not return a proper error response, which might expose database internals or other sensitive information to clients.  Instead, the program might crash or exhibit unexpected behavior. 

## Solution
The `bugSolution.js` file shows the corrected code, demonstrating how to handle missing users gracefully by returning a 404 status code.