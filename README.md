# MongoDB $inc Operator Issue

This repository demonstrates a common issue encountered when using the `$inc` operator in MongoDB update queries.  Specifically, it highlights the unexpected behavior that occurs when attempting to increment/decrement a field that does not yet exist in the document.

The `bug.js` file showcases the problematic code, and `bugSolution.js` provides a corrected version.

## Problem
The issue lies in silently failing to increment/decrement a field that doesn't exist rather than throwing an error.