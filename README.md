# Unexpected Routing Behavior with Nested Routes and Wildcard Route in React Router v6

This repository demonstrates an unexpected routing behavior in React Router v6 when using nested routes in conjunction with a wildcard route ('*').  When a wildcard route is present, nested routes might not behave as expected, causing incorrect page rendering.

## Bug Description:

In the `App.js` file, the application uses nested routes.  However, due to the presence of the wildcard route `path="*"`, the nested route `/about/contact` fails to render correctly. Instead, the `NotFound` component is rendered.

## Solution:

The solution involves re-structuring the routes to avoid the conflict between the nested route and the wildcard route, ensuring the correct rendering of nested components.
The `AppSolution.js` file demonstrates the corrected routing structure.