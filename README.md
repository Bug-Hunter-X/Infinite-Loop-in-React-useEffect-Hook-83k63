# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The example shows how an incorrect dependency array can lead to an infinite rendering loop.

## The Problem
The `useEffect` hook is designed to perform side effects after a component renders.  However, if the dependency array is missing or incorrect, the effect function might run unexpectedly, causing performance issues or even crashes.

In this case, a missing dependency in the `useEffect` hook's dependency array causes an infinite loop.

## How to Reproduce
Clone this repository and run `npm start`.

## Solution
The solution involves correctly specifying the dependencies in the `useEffect` hook's dependency array.  By including only the necessary state variables, you ensure that the effect function only runs when those variables change.