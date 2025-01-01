# Tailwind CSS Vertical Centering Bug

This repository demonstrates a common issue encountered when attempting to vertically center elements using Tailwind CSS's flexbox utilities.  The problem arises from a misunderstanding of how `justify-center` and `items-center` interact with parent container dimensions.

## The Bug

The provided `bug.js` file contains code that aims to center a button both horizontally and vertically within its parent container using `flex`, `justify-center`, and `items-center`. However, the button may not be vertically centered as expected. This is because the parent container's height is implicitly determined by its contents, potentially preventing proper vertical centering.

## The Solution

The `bugSolution.js` file offers a solution by explicitly setting the parent container's height (e.g., using `h-screen`, `h-[100px]`, or other appropriate height setting) or applying a different strategy like using `grid` layout and aligning items.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` (or similar file in your setup). 
3. Observe that the button is not perfectly vertically centered.
4. Then open `bugSolution.html` to see the corrected version.