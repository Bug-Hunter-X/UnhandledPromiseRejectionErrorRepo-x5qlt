# Unhandled Promise Rejection: Cannot read properties of undefined (reading '...') in React Native

This repository demonstrates a common React Native bug related to accessing state variables before they've been initialized.  The problem arises from asynchronous operations where the state hasn't been updated yet when the component renders. This often manifests as an `Unhandled Promise Rejection` error.

## Bug Description
The `Bug.js` file shows an example of this issue, where we try to render data from an API before the API call completes.

## Solution
The `BugSolution.js` file demonstrates how to resolve this using the `useEffect` hook and conditional rendering. By checking if the state variable is defined, we avoid errors until the data is available.

## How to run the example:
1. Clone this repository
2. Navigate to the project folder
3. Run `npm install`
4. Run `npx react-native run-android` or `npx react-native run-ios` depending on your environment