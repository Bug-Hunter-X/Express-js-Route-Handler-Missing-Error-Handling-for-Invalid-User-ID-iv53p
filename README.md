# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling when dealing with user inputs.  Specifically, the example shows a route that fetches a user by ID but fails to handle cases where the ID is not a valid integer. This can lead to unexpected errors or crashes.

## Bug

The `bug.js` file contains the faulty code.  It attempts to parse the user ID as an integer using `parseInt()`, but doesn't include any error handling if the ID cannot be parsed.

## Solution

The `bugSolution.js` file provides a corrected version. It includes error handling to catch cases where the ID is not a valid integer, returning an appropriate HTTP error response if necessary.