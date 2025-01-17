# Uncommon HTML Error: Accessing Non-Existent Attributes

This repository demonstrates an uncommon HTML error related to accessing non-existent attributes of HTML elements.  While this may not always result in a JavaScript error, it can lead to subtle bugs and unexpected behavior in your web application.

The `bug.html` file contains the erroneous code. The `bugSolution.html` provides a corrected version.

## Description
The bug arises from attempting to access an attribute that doesn't exist on an HTML element.  Many browsers handle this gracefully by returning `undefined`, but this can still cause unexpected behavior or silent failures down the line, especially in larger applications.

## How to reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the console (usually accessed by pressing F12). While no explicit error is thrown, the behavior may be unexpected, depending on how the undefined value is used.

## Solution
The best practice is to always check for the existence of an attribute before attempting to access its value.

The corrected code in `bugSolution.html` uses an explicit check to avoid any issues.
