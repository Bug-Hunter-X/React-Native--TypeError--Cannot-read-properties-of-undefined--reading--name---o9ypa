# React Native: Handling Asynchronous Data and Preventing 'Cannot read properties of undefined' Errors

This repository demonstrates a common error in React Native development and its solution. The error, `TypeError: Cannot read properties of undefined (reading 'name')`, arises when trying to access a property of an object before it's properly loaded from an asynchronous operation, such as a network request.

## Problem
The `bug.js` file showcases the problematic code.  It attempts to render data from an API call before the call has finished, resulting in the error.  This is a frequent issue when dealing with asynchronous data fetching in React Native applications.

## Solution
The `bugSolution.js` file presents a solution by implementing optional chaining (`?.`) and nullish coalescing (`??`). These operators provide a concise way to handle the possibility of `null` or `undefined` values, preventing the error.  The code also includes error handling for more robust behavior.

## How to Run
1. Clone this repository.
2. Navigate to the project directory in your terminal.
3. Run `npm install` or `yarn install` to install the necessary packages.
4. Run `npx react-native run-android` or `npx react-native run-ios` to start the app in your emulator or device.