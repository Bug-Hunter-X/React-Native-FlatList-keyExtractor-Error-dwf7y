# React Native FlatList `keyExtractor` Error

This repository demonstrates a common error encountered when using the `FlatList` component in React Native: incorrectly implementing the `keyExtractor` prop.  Using the index as the key is problematic because it can lead to incorrect rendering and performance issues when the data array is modified.

## The Problem

The `keyExtractor` prop in `FlatList` requires a function that returns a unique string key for each item in the data array.  If you use the index as the key, React Native might not correctly update the list when items are added, removed, or reordered.

## The Solution

Always use a unique identifier from each item in your data array as the key.  This ensures that React Native can efficiently update the list when data changes.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run the app on an emulator or device.
4. Observe the incorrect rendering when the data changes.
5. Refer to `bugSolution.js` to see the correct implementation.
