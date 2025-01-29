# React useEffect Hook Missing Return Statement

This repository demonstrates a common but easily overlooked error in React's `useEffect` hook: the missing return statement for cleanup functions.  Forgetting to include a return statement within `useEffect` can lead to memory leaks and unexpected behavior, especially when dealing with event listeners, timers, or subscriptions.

The `bug.js` file showcases the problematic code, while `bugSolution.js` provides the corrected version.  The key difference lies in the addition of a return statement within the `useEffect` function that performs necessary cleanup actions before the component unmounts.