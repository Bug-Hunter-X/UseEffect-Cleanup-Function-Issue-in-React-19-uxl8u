# React 19 useEffect Cleanup Function Issue
This repository demonstrates a common issue with the `useEffect` hook's cleanup function in React 19.  The example shows an interval that is not properly cleared, leading to a memory leak.

## Bug
The `bug.js` file contains a component that uses `useEffect` to set up an interval. However, the cleanup function is not correctly implemented which causes the interval to continue even after the component unmounts.

## Solution
The `bugSolution.js` file shows the corrected implementation where the `clearInterval` function is correctly used to clear the interval within the cleanup function, preventing memory leaks.

## How to run
1. Clone the repository
2. Navigate to the repository directory in the terminal
3. Run `npm install`
4. Run `npm start`
