# Uncommon HTML Event Listener Bug

This repository demonstrates an uncommon issue related to adding multiple event listeners to a single HTML element.  The problem arises from using both the traditional assignment method (`onclick = function(){...}`) and the `addEventListener` method simultaneously. This can lead to the event handler firing multiple times or behaving unpredictably.

The `bug.html` file showcases the problem. The `bugSolution.html` file shows how to correct the behavior.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Click on the div element.

You'll notice that the alert box pops up twice. This demonstrates the unexpected behavior caused by the combination of both event listener assignment methods.

## Solution

The `bugSolution.html` file shows the correct approach: use either `onclick` or `addEventListener`, but not both for the same event on the same element. This prevents unintended multiple executions of the event handler function.