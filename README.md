# React useEffect Hook Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug occurs when the dependency array is missing or incomplete, leading to an infinite render loop.

## Bug Description

The `useEffect` hook, without a correctly specified dependency array, re-renders the component continuously because it lacks the criteria to detect state changes. This results in an infinite loop and performance issues. The provided example shows this behavior using the `count` state variable.

## Solution

The solution involves properly specifying the dependencies in the dependency array.  By including `count` in the array, the effect only runs when the value of `count` changes.