# CSS `calc()` Issue in Flexbox

This repository demonstrates a common issue when using the `calc()` function in CSS within a flexbox context. The problem arises from the way `calc()` interacts with percentage values within flex items. Percentages are calculated relative to the available space in the flex container, not the overall parent element width.  This can lead to unexpected results, especially when the flex container has margins or padding.

The `bug.css` file shows the erroneous code, and `bugSolution.css` provides the corrected implementation.

## How to Reproduce

1. Clone this repository.
2. Open `index.html` (you'll need to create this simple HTML file that includes the CSS). 
3. Observe the incorrect width of the flex item in the first example.
4. Compare it to the correct width in the second example.

## Solution

The solution might involve adjusting the flexbox container's dimensions, accounting for padding/margin in the `calc()` function, or using a different approach to achieve the desired layout.