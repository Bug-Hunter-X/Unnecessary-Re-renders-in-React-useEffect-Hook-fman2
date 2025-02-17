# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common React issue where the `useEffect` hook causes unnecessary re-renders due to its execution after every render cycle. The provided solution uses `useCallback` to optimize performance. 

## Bug
The `bug.js` file shows a component that logs the count to the console after every render, regardless of whether the count has actually changed. This leads to performance degradation, particularly with more complex components and state updates.

## Solution
The `bugSolution.js` file demonstrates how to solve the problem by using `useCallback` to memoize the effect function. This ensures the effect only runs when the count value changes, significantly improving performance and reducing unnecessary console logs.