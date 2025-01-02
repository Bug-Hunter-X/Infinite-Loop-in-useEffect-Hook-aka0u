# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: creating an infinite loop within the `useEffect` hook.

The `bug.js` file contains a component that attempts to increment a state variable within its own `useEffect` dependency array, leading to continuous re-renders and an infinite loop.  The `bugSolution.js` file provides a corrected version.

**Key Learning:**  Avoid updating state variables within the dependency array of a `useEffect` hook that the state variable is part of unless you are implementing advanced state management techniques that handle this case correctly.