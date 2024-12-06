# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js: unhandled exceptions within an HTTP server.  The `bug.js` file shows an example where an exception is thrown without proper handling, causing the server to crash. The `bugSolution.js` file provides a corrected version with improved error handling.

## Problem

The original code throws an error without a `try...catch` block within the request handler, resulting in an unhandled exception and server termination.

## Solution

The solution uses a `try...catch` block to gracefully handle the exception, preventing the server from crashing.  It also logs the error for debugging purposes.  This allows the server to continue operating even if an unexpected error occurs.