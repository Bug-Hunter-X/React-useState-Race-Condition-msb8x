# React useState Race Condition

This repository demonstrates a common issue in React applications involving the `useState` hook and race conditions.  When you update the state multiple times within a single event handler, the updates might not apply sequentially, leading to unexpected results.  This example showcases how calling `setCount` twice in quick succession creates a race condition, resulting in a count that might not increase by the expected amount.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Click the 'Increment' button multiple times and observe the inconsistencies in count updates.

## Solution

The solution involves updating the state using a functional approach to ensure the latest state value is considered during the update. This eliminates the race condition and ensures consistent state updates. The solution code shows this improvement.
