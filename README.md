# Next.js 15 Production Build Error: Unhandled Runtime Error

This repository demonstrates a common issue in Next.js 15 production builds where unhandled runtime errors in page components cause the entire application to crash.  The error only surfaces in the production build, not during development.

## Problem

The `pages/about.js` file attempts to access a property that does not exist, resulting in a runtime error. This error is gracefully handled during development, but in production it leads to a blank page or a server error.

## Solution

The solution involves robust error handling using try...catch blocks to prevent the application from crashing.  This ensures a more user-friendly experience even when unexpected errors occur.