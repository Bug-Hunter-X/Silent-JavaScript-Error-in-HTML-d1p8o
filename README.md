# Silent JavaScript Error in HTML

This repository demonstrates an uncommon HTML/JavaScript bug where a JavaScript error is silently ignored by the browser. The script tries to access a non-existent element, leading to an error that is not displayed in the browser's console.  This can make debugging difficult.

## Bug Description

The `bug.html` file contains a script that attempts to modify the `innerHTML` of a non-existent element.  This action normally throws a `TypeError` in JavaScript. However, without proper error handling (try...catch),  modern browsers may swallow this error without providing any indication of the issue to the developer.

## Solution

The `bugSolution.html` file shows the corrected code using a `try...catch` block to handle potential errors. This will allow you to see the error in the browser's console, which makes debugging easier.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Open the browser's developer console (usually by pressing F12).
4. You will likely see no error messages despite the script having a problem.
5. Now open `bugSolution.html`. 
6. Open the browser's developer console and you should observe a clear error message related to the missing element. 
