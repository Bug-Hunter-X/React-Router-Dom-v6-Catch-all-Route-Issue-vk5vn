# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using the catch-all route `/*` in React Router DOM v6. The catch-all route, intended to handle any unmatched paths, is unexpectedly overriding other more specific routes.

## Problem

The provided `App.js` demonstrates a scenario where the catch-all route `/*` is preventing the `/about` route from functioning.  Navigating to `/about` should show the About component but instead displays the NotFound component.

## Solution

The solution, shown in `AppSolution.js`, involves moving the catch-all route to be the last route defined in the `Routes` component.