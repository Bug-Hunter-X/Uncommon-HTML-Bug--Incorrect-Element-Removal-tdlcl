# Uncommon HTML Bug: Incorrect Element Removal

This repository demonstrates a subtle but important bug related to element removal in HTML.
The bug involves using `innerHTML` to remove an element from the DOM, which unexpectedly removes the element completely and not just its content. The correct way to remove an element is using `removeChild()`.

## Bug Description
The `bug.html` file contains a div with some text inside it. A JavaScript script attempts to remove the text within the div element using `innerHTML = "";` however, this removes the entire div, not just its content.

## Solution
The `bugSolution.html` file demonstrates the correct approach, which is to use `removeChild()` to remove the element, preserving the overall DOM structure.

## How to reproduce
1. Open `bug.html` in your browser.
2. Observe that the div element is removed completely after the script executes.
3. Open `bugSolution.html` in your browser.
4. Notice the div element is removed correctly, without any unexpected side effects.