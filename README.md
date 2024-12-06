# React Native FlatList KeyExtractor Bug

This repository demonstrates a common bug in React Native's FlatList component: using a `keyExtractor` function that doesn't return unique keys for each item in the data array.  This can lead to unexpected rendering behavior and performance issues.

## Bug Description
The `bug.js` file contains a FlatList with duplicate keys, causing incorrect rendering of list items.  The solution is demonstrated in `bugSolution.js`.

## How to reproduce
1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app on a simulator or device.
4. Observe the incorrect rendering of the list items in `bug.js`.
5. Compare with the corrected rendering in `bugSolution.js`

## Solution
The solution involves ensuring the `keyExtractor` function always returns a unique identifier for each item.  The best practice is to use a unique identifier from your data source, such as an ID or UUID.