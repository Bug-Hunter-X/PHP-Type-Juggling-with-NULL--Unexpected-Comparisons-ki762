# PHP Type Juggling with NULL: Unexpected Comparisons

This repository demonstrates a common, yet subtle, error in PHP related to type juggling and comparisons involving `NULL`.  PHP's loose comparison operator (`==`) can lead to unexpected results when comparing `NULL` to `0` or an empty string.

The `bug.php` file showcases this issue. The `bugSolution.php` file provides a corrected version using strict comparison (`===`) to avoid type juggling and ensure accurate comparisons.

## How to Reproduce

1. Clone this repository.
2. Run `bug.php` using a PHP interpreter.
3. Observe the unexpected output.
4. Run `bugSolution.php` to see the corrected behavior using strict comparison.

## Solution

Always use strict comparison (`===`) when comparing values in PHP, especially when dealing with `NULL`, to prevent type juggling and ensure accurate comparisons.  Strict comparison checks for both value and type equality.