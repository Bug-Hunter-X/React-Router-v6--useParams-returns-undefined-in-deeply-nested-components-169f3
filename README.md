# React Router v6 useParams Issue in Nested Routes

This repository demonstrates a common issue encountered when using the `useParams` hook in React Router v6 within deeply nested components.  The issue is that despite the route matching correctly, the `useParams` hook may return `undefined` values for the parameters.

The `NestedRoutesBug.js` file shows the problematic implementation, while `NestedRoutesSolution.js` provides a working solution.

## Problem
In deeply nested component structures, React's reconciliation process and the way React Router updates its internal state can sometimes lead to incorrect parameter propagation. The `useParams` hook might not receive the updated parameters immediately after navigation.