# React Memory Leak: Unclosed setInterval in useEffect

This repository demonstrates a common React bug: a memory leak caused by improper usage of the `setInterval` function within the `useEffect` hook.  The provided `bug.js` file contains the faulty code, resulting in a continuously running interval that is never cleared.

The solution, `bugSolution.js`, demonstrates how to correctly handle the interval and prevent the memory leak by using the cleanup function provided by `useEffect`.