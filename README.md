# Next.js 15 - useState Hook Error Outside Functional Component

This repository demonstrates a subtle error that can occur in Next.js 15 applications when using the `useState` hook outside of a functional component.  The error isn't always immediately obvious and might require careful debugging.

## Problem

The `useState` hook is designed for use within functional components.  If you inadvertently attempt to use it elsewhere (e.g., in a regular JavaScript file or a class component), you'll encounter an error.  Next.js's error handling might not always clearly pinpoint the source of the problem.

## Solution

Ensure that all uses of the `useState` hook are contained within functional components.  Refactor your code to adhere to this rule. If you need state management outside of functional components, consider using Context API or a state management library like Redux or Zustand.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about`.
5. Observe the error in your console.