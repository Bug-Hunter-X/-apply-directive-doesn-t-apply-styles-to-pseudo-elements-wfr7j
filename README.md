# Bug Report: @apply Directive and Pseudo-elements in Tailwind CSS

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles defined for pseudo-elements (`:before` and `:after`) when used within a custom class.  The issue arises because the `@apply` directive doesn't correctly handle the pseudo-element selectors.

## Steps to Reproduce

1. Include the `bug.css` stylesheet in your project.
2. Observe that the expected pseudo-element styles are missing.
3. Compare with `bugSolution.css` for the corrected approach.

## Expected Behavior

The `@apply` directive should correctly apply styles defined for pseudo-elements, including the `::before` and `::after` selectors.

## Actual Behavior

The pseudo-element styles are not applied when using `@apply`.

## Workaround

The provided `bugSolution.css` showcases a workaround using direct application of styles instead of `@apply`.

## Solution

This bug is related to the way `@apply` handles complex selectors.  A proper fix requires improvements in Tailwind's `@apply` functionality to handle pseudo-element selectors correctly.  Until a fix is implemented, the workaround should be used.