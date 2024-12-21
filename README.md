# React Native useState Hook Not Updating UI When Modifying Object/Array Directly

This repository demonstrates a common issue in React Native development where the `useState` hook doesn't correctly update the UI when an object or array in the state is modified directly.  The problem lies in how JavaScript handles object/array mutations. Directly modifying properties within the object or array does not trigger a re-render because the reference to the object/array in the state remains unchanged.

The `bug.js` file shows the buggy code, illustrating the incorrect approach.  The `bugSolution.js` file offers solutions to correctly update the UI by creating copies of the object/array before making changes using spread syntax or other methods.