# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6.  The catch-all route is intended to handle any unmatched routes, but in this example, it's not functioning correctly.

## Problem

The provided `App.js` shows a basic React Router setup.  Routes for `/` and `/about` work as expected.  However, the `/*` route, intended to act as a 404 Not Found page, never gets triggered, even when navigating to an invalid path. 

## Solution

The solution involves re-ordering the routes. The catch-all route must be defined last, below any other specific routes, for it to catch any unmatched routes.