# React Router v6 Catch-all Route Bug

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router v6. The problem is that the catch-all route always matches, overriding other routes which should take precedence.  This example shows the problem and how to solve it.

## Problem:

The provided `App.js` uses a catch-all route which overshadows other routes, preventing access to pages like '/about'.

## Solution:

The `AppSolution.js` file provides a corrected version.  The solution involves placing the catch-all route as the last route within the `Routes` component. This ensures that it only matches if no other routes are matched first. 