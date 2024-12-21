# Express.js Unhandled Error
This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  Specifically, the `/users/:id` route fails to handle cases where a user with the given ID does not exist.

## Bug
The `bug.js` file contains an Express.js route handler that fetches a user by ID.  It lacks error handling for when a user with the specified ID is not found, potentially leading to unexpected behavior or crashes.

## Solution
The `bugSolution.js` file demonstrates the correct way to handle this situation, adding a check for the existence of the user and returning an appropriate response (404 Not Found) if the user is not found.

## How to reproduce
1. Clone this repository.
2. Run `npm install express`.
3. Run the `bug.js` file using Node.js.  Try accessing a non-existent user ID. 
4. Run the `bugSolution.js` file to see the correct implementation.
