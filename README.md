# React useEffect Hook Bug
This repository demonstrates a common bug in React's `useEffect` hook: an infinite loop caused by a missing dependency.

## The Bug
The `bug.js` file contains a component that uses the `useEffect` hook to log the current count to the console. However, the `count` variable is not included in the dependency array, causing the effect to run on every render, leading to an infinite loop and performance issues.

## The Solution
The `bugSolution.js` file fixes this bug by adding `count` to the dependency array. This ensures that the effect only runs when the `count` value changes.

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console and see the infinite loop in the original version. Then, switch to the solution and observe the fixed version.