# Unexpected NaN Comparison in JavaScript

This example demonstrates the unexpected behavior of JavaScript's comparison operators when dealing with `NaN` (Not a Number).

## The Bug

The function `foo` attempts to compare two numbers using strict equality (`===`). However, when both inputs are `NaN`, it incorrectly returns `false`, even though `NaN` is never equal to itself.

## The Solution

The solution involves using `Number.isNaN()` to check if a value is `NaN` before performing any comparisons. This ensures the correct behavior when handling `NaN` values.