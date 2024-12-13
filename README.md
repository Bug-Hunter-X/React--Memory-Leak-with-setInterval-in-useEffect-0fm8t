# React: Memory Leak with setInterval in useEffect

This repository demonstrates a common React bug involving memory leaks caused by the improper use of `setInterval` within the `useEffect` hook.

The `bug.js` file shows the erroneous implementation.  The `setInterval` function is called without a cleanup function, resulting in multiple intervals running indefinitely, leading to memory leaks and performance issues.

The `bugSolution.js` file presents the corrected implementation with a proper cleanup function using `clearInterval`.  This ensures that the interval is cleared when the component unmounts or when the effect dependencies change, preventing memory leaks.
