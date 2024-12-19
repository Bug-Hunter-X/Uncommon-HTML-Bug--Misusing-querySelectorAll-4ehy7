# Uncommon HTML Bug: Misusing querySelectorAll

This repository demonstrates a subtle but important distinction in how to select elements using `querySelectorAll` vs. `querySelector` in JavaScript when interacting with HTML.

The `bug.html` file showcases the incorrect usage of `querySelectorAll` when attempting to select a single element identified by its ID.  The correct approach, using `querySelector`, is shown in `bugSolution.html`.

## The Bug

The incorrect code uses `querySelectorAll` to select an element with a specific ID.  While this works in some cases, it's inefficient and can lead to unexpected behavior, particularly if you're not carefully handling the NodeList that's returned.

## The Solution

The solution highlights the more efficient and straightforward method: using `querySelector` to directly select the element by its ID. This returns the element directly, avoiding the need to access a specific index in a NodeList.