# React useEffect Runs on Every Render

This repository demonstrates a common mistake in React's `useEffect` hook: forgetting to specify the dependency array correctly.  When the dependency array is omitted or incorrect, the effect runs after every render, not just when dependencies change.  This can lead to performance problems and unexpected behavior.

## Bug
The `bug.js` file shows an example of this. The `useEffect` hook logs a message to the console on every render, causing unnecessary console output and potential performance issues in more complex components.

## Solution
The `bugSolution.js` file demonstrates the correct way to use `useEffect`. The dependency array `[count]` ensures the effect runs only when the `count` variable changes. This improves performance and avoids unexpected behavior.

This example highlights the importance of careful consideration when constructing dependency arrays within React's `useEffect` hook.