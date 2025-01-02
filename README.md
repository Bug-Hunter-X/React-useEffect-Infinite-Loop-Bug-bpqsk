# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The provided code exhibits an infinite loop due to a missing dependency in the `useEffect` function. The solution demonstrates the correct way to resolve this issue by including `count` in the dependency array.  This ensures the effect only runs when the value of count changes.

## Bug
The bug lies within the `useEffect` hook in `MyComponent`.  Because `count` is not listed in the dependency array, the effect will run after every render, leading to an infinite loop and causing a crash or significant performance degradation in the browser console.