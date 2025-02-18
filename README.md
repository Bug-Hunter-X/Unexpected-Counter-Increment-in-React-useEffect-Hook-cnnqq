# React useEffect Hook with setInterval Bug

This repository demonstrates a common bug in React's `useEffect` hook when using `setInterval`.  The counter is supposed to increment every second, but it increments rapidly. This is because the `setInterval` is called repeatedly, which leads to unintended behavior.

## Bug Description
The provided `bug.js` file shows an implementation of `useEffect` with `setInterval`. The intention is to update the counter every 1000 milliseconds. However, due to the way the `useEffect` hook is used, the `setInterval` is invoked continuously, which leads to a very rapid increase of the counter value.

## Solution
The solution demonstrates the correct implementation.  The `useEffect` hook is used properly, with the `setInterval` only being initialized once.

## How to Reproduce
1. Clone the repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npm start` to start the development server.
4. Observe the unexpected counter behavior in `bug.js` and the correct behavior in `bugSolution.js`.
