# React useEffect Cleanup Function Issue

This repository demonstrates a common, yet often subtle, bug related to the cleanup function in React's `useEffect` hook.  The issue arises from a misunderstanding of how the dependency array works and can lead to memory leaks or unexpected behavior.

## Bug Description:

The provided code implements a simple counter component. An `useEffect` hook is used to log messages to the console both during rendering and before unmounting.  However, in some situations, the cleanup function might not run as expected. 

## Solution:

The solution addresses the core issue by ensuring that the useEffect function will always run its cleanup routine before component unmounts. 

## How to Reproduce:

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs.
