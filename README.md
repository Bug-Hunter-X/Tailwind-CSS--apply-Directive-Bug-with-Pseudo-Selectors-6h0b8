# Tailwind CSS @apply Directive Bug with Pseudo-Selectors

This repository demonstrates a bug in Tailwind CSS where the `@apply` directive does not correctly apply styles when pseudo-selectors like `:hover` or `:focus` are used.  This results in unexpected visual behavior that deviates from the intended design.

## Bug Description

When using `@apply` with a class containing pseudo-selectors, only the base styles are applied, while the pseudo-selector styles are ignored. This issue can be particularly problematic for interactive elements where hover or focus states are crucial for user experience.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install` to install the necessary dependencies.
3. Open `index.html` in your browser.  Observe that the hover effect on the button is not applied as expected.

## Solution

Instead of using `@apply` with pseudo-selectors, apply them directly in the HTML class.  This ensures that Tailwind processes them correctly.