# CSS Pseudo-element Overlap Bug

This repository demonstrates an unusual CSS bug where a `::before` pseudo-element overlaps its parent element's content. The problem stems from either improper `z-index` management or the absence of a proper stacking context.

## Bug Description

A `::before` pseudo-element is used to display text over a parent element. However, even with a seemingly correct `z-index`, the pseudo-element unexpectedly overlaps the main content. This behavior highlights the complexities of stacking context in CSS.   See `bug.css` for the problematic code.

## Solution

The solution involves creating a proper stacking context for the parent element and ensuring that the `z-index` values are correctly set to establish the desired stacking order. This is demonstrated in `bugSolution.css`. 