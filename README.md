# CSS Specificity Gotcha: Unexpected Selector Precedence

This repository demonstrates a subtle issue related to CSS specificity.  A more specific class selector unexpectedly overrides an ID selector due to the way inheritance and the cascade interact. This is a common error for developers less familiar with the nuances of CSS specificity.

The `bug.css` file showcases the issue. `bugSolution.css` offers a corrected version.

## Understanding the Issue

CSS specificity determines which style rules apply when multiple rules target the same element.  Generally, ID selectors have the highest specificity, followed by class selectors, and then element selectors. However, the interaction between inheritance and the cascade can lead to unexpected behavior if not carefully considered.