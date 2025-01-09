# useEffect Hook with Empty Dependency Array Issue in React 19

This repository demonstrates an uncommon bug related to the `useEffect` hook with an empty dependency array in React 19.  The issue arises when you expect a component to re-render based on state changes, but it doesn't due to the effect only running once on mount.

## Bug Description

The `useEffect` hook with an empty dependency array (`[]`) is designed to run only once after the initial render. However, if you intend for the effect to run whenever certain state variables change,  using an empty array will prevent the desired behavior.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe that the counter does not update even after clicking the button. 