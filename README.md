# Uncommon HTML Bug: Element Disappears After Button Click

This repository demonstrates a subtle bug in HTML where an element disappears after a button click and is not re-displayed.  The bug is caused by a missing piece of code to toggle the visibility of the element.

The `bug.html` file shows the problematic code.  The `bugSolution.html` file provides the corrected code.

## Bug Description:
The button click event handler hides the div element using `style.display = "none";`. However, there's no code to make the div reappear.  This causes the div to remain permanently hidden after the first click.

## Solution:
The solution involves adding a simple check to toggle the visibility.  If the element is visible, set its display property to "none"; if it's hidden, set it to "block".