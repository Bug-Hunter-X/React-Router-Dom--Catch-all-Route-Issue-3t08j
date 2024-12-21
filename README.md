# React Router Dom Catch-all Route Issue
This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router Dom v6. The catch-all route unexpectedly matches before other, more specific routes, leading to incorrect component rendering.

## Problem
The issue arises when a catch-all route (`/*`) is placed after more specific routes.  Even if a path matches a more specific route, the catch-all route will still be triggered, overriding the intended component.

## Solution
To fix this, the catch-all route should always be placed as the last route defined within the `<Routes>` component.