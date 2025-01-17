# CSS Specificity and Inheritance Conflict

This repository demonstrates an uncommon issue in CSS related to specificity and inheritance.  A less specific rule can sometimes override a more specific one if certain conditions regarding inheritance and declaration order are met.  The `bug.css` file contains the problematic code, while `bugSolution.css` offers a solution.

## Bug Description

A more specific CSS selector (e.g., `div p`) might not apply its styles if a less specific selector (`p`) has already declared a style for the same inherited property.

## Solution

The solution file shows how to structure the CSS to ensure the intended behavior and solve the specificity issue.  This usually involves carefully ordering rules or using the `!important` flag (though using `!important` should be avoided if possible).