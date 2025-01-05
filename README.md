# Unhandled Network Error in React Native Fetch API

This repository demonstrates a common issue in React Native applications: unhandled network errors when using the Fetch API.  The `DataList.js` file shows the problematic code, while `DataListSolution.js` provides a robust solution.

## Problem

The initial code lacks proper error handling within the `fetch` call.  Network errors (like a server being down) are not caught, leading to a silent failure or a crash in the app.

## Solution

The solution introduces a `try...catch` block to handle potential errors during the fetch operation.  A `finally` block ensures the `loading` state is updated, providing user feedback regardless of success or failure.  Error messages are displayed to inform the user about the problem.