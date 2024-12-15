# React setInterval Memory Leak

This example demonstrates a common mistake when using `setInterval` within a React component: forgetting to clear the interval when the component unmounts. This leads to a memory leak, as the interval continues to run even after the component is no longer needed.

The `bug.js` file contains the buggy code.  The solution, which includes a cleanup function to clear the interval using `clearInterval`, is in `bugSolution.js`.