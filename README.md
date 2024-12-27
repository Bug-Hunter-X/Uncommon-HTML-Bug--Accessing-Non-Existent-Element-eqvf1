# Uncommon HTML Bug: Accessing Non-Existent Element

This repository demonstrates a common, yet often overlooked, error in HTML/JavaScript: attempting to access an element in the DOM that does not yet exist or has not been properly rendered.  The issue frequently occurs when scripts execute before the elements they reference have been parsed by the browser.

The `bug.html` file shows the erroneous code. The `bugSolution.html` provides the correct approach.

## How to Reproduce

1. Open `bug.html` in your web browser.
2. Observe the error in your browser's developer console.

## Solution

The solution involves ensuring that the script accessing the element runs only *after* the element is ready. This can be achieved through several methods including event listeners or using a `DOMContentLoaded` event listener. Refer to `bugSolution.html` for the corrected code.