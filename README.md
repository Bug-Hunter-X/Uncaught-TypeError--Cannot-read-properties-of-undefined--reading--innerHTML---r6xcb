# Uncommon HTML Error: Accessing Non-Existent Element Properties

This repository demonstrates a subtle but potentially problematic error in JavaScript code embedded within an HTML file. The error occurs when attempting to access a property of a DOM element before verifying that the element actually exists.

## The Bug

The `bug.html` file contains a script that tries to set the `innerHTML` property of an element with the id "myDiv."  However, it doesn't first check if `document.getElementById("myDiv")` returns a valid element. If the element doesn't exist, this will result in a runtime error.

## The Solution

The `bugSolution.html` file shows the corrected code. It includes a check to ensure the element exists before attempting to modify its properties. This prevents the error and improves the robustness of the code.