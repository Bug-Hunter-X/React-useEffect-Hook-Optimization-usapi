# React useEffect Hook Optimization

This repository demonstrates a common performance issue in React applications caused by inefficient use of the `useEffect` hook and provides a solution.

## Problem

The `useEffect` hook in the provided `MyComponent` runs after every render, causing unnecessary re-renders and potential performance issues if the component is frequently updated.  This is because the dependency array is missing or not properly specified.

## Solution

The solution utilizes the dependency array within the `useEffect` hook to precisely control when it re-runs. By including `count` in the dependency array, the effect only runs when `count` changes.

## How to use

1. Clone the repository.
2. Navigate to the cloned directory.
3. Run `npm install` to install the dependencies.
4. Run `npm start` to start the development server.