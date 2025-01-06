# CSS Calc() Calculation Error

This repository demonstrates a common error encountered when using the `calc()` function in CSS. The problem arises from misinterpreting how `calc()` interacts with the context of its parent element's size and inheritance.

The `bug.css` file showcases the incorrect implementation, and `solution.css` provides a corrected version.

## Problem Description

The `calc()` function is powerful, but its results rely on the dimensions of the parent element. If the parent element's dimensions are undefined or dynamically changing, the calculation in the child element may not yield the expected outcome.

## Solution

Ensure that the parent element has defined dimensions (using `width` and `height` properties) or uses a layout technique that ensures its size is predictable before relying on `calc()` within its children for accurate calculations. Consider using viewport units (`vw`, `vh`) if the calculation needs to relate to the browser window size instead of a parent's dimensions.
