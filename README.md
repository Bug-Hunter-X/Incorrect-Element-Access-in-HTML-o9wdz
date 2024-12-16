# Incorrect Element Access in HTML
This repository demonstrates a common yet easily overlooked error in accessing HTML elements using JavaScript.
The issue arises from incorrectly using the `document.getElementById()` method. The '#' symbol is not necessary and including it results in failure to select the intended element, leading to unexpected behavior in the application.
The bug.html file shows the incorrect implementation, while bugSolution.html provides the correct implementation.
## Bug Description
The bug is in the JavaScript code within the HTML file.  Specifically, the line `var element = document.getElementById('#myDiv');` is wrong.  `getElementById` expects only the ID of the element, not a selector string beginning with '#'. This leads to the script failing to find the element and returning 'null'.
## Solution
The bug is fixed by removing the '#' character in `document.getElementById()` call to properly target the element.