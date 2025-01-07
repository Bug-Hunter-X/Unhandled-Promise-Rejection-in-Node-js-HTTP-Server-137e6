# Unhandled Promise Rejection in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: unhandled promise rejections in HTTP servers.  The `bug.js` file shows a server that handles asynchronous operations but lacks robust error handling.  The `bugSolution.js` file provides a corrected version with improved error handling.

## Problem

The original code simulates an asynchronous operation that might fail. If the operation fails, the error is logged to the console, but the HTTP response is incomplete and lacks details about the error.  This can lead to unexpected behavior and make debugging difficult.

## Solution

The solution demonstrates how to properly handle promise rejections in an HTTP server.  It includes a more comprehensive `try...catch` block to manage potential errors and sends a more informative error response to the client.