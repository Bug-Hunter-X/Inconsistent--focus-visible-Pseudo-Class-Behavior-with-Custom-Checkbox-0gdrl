# Inconsistent :focus-visible Pseudo-Class Behavior with Custom Checkbox

This repository demonstrates an uncommon issue with the CSS `:focus-visible` pseudo-class when used with a custom checkbox element. The goal is for the checkbox to have a visible focus outline *only* when focused using the keyboard (not mouse clicks). However, inconsistencies across browsers and potential interference from other CSS or JavaScript can cause the outline to appear on mouse focus as well.

## Problem

The primary issue lies in the reliability of the `:focus-visible` pseudo-class.  While designed to improve user experience by reducing visual clutter on mouse clicks, its implementation can be inconsistent across different browsers and environments.

## Solution (Partial)

Unfortunately, a perfect, cross-browser solution that guarantees consistent `:focus-visible` behavior is not always possible due to limitations in browser implementation. However, techniques can be attempted to mitigate the issue. See `bugSolution.css` for possible mitigation approaches.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` (create a simple html file that includes `bug.css` and a checkbox). 
3. Observe the focus outline's behavior when interacting with the checkbox using both mouse clicks and keyboard navigation.
4. Compare the behavior with different browsers to highlight the inconsistencies.
