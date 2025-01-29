# Incorrect Usage of getElementsByTagName with innerHTML

This repository demonstrates a common error when working with the `getElementsByTagName` method in JavaScript within an HTML context.

The issue arises from attempting to directly modify the `innerHTML` property of the HTMLCollection returned by `getElementsByTagName`.  `getElementsByTagName` returns a collection of elements, not a single element, so `innerHTML` is not a property of the collection itself.  To modify the content, you need to iterate through the collection and update each element individually.

The `bug.html` file contains the erroneous code.  The `bugSolution.html` file provides the corrected version.
