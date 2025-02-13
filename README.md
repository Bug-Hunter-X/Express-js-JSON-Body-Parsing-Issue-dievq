# Express.js JSON Body Parsing Issue

This repository demonstrates a common issue in Express.js applications where JSON request bodies are not parsed correctly if the `Content-Type` header is missing or incorrect.  The bug and solution are outlined below.

## Bug
The provided `bug.js` file shows an Express.js server designed to receive JSON data.  However, if a client sends a POST request without setting the `Content-Type` header to `application/json`, the `req.body` will be empty. This leads to unexpected behavior or errors in the application.

## Solution
The `bugSolution.js` file provides a corrected version.  It incorporates stricter input validation and ensures proper handling of potentially missing or malformed JSON data in the request body, thus solving the issue.