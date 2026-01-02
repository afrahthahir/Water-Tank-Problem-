# Water Tank Problem - Web Application

This repository contains a frontend solution for the **Water Tank Problem** (Trapping Rain Water), built as an interview assignment.

## Problem Description

Given an array of non-negative integers representing the heights of blocks, the goal is to compute how many units of water can be trapped between these blocks.

**Input**: An array of integers, e.g., `[0,4,0,0,0,6,0,6,4,0]`.

**Output**: The total units of water stored (e.g., **18 Units**).



## The Approach: Two-Pointer Technique

To solve this efficiently, I implemented the **Two-Pointer Algorithm**. This approach is optimal for performance, operating in  time complexity and  space complexity.

### Logic Summary:

1. **Initialize**: Two pointers, `left` (start of the array) and `right` (end of the array).
2. **Tracking**: We maintain `leftMax` and `rightMax` variables to store the tallest boundary encountered from either side.
3. **Calculation**:
* We compare the heights at the `left` and `right` pointers.
* Water levels are determined by the **shorter** of the two boundaries, as water cannot rise above the lowest wall.
* If the current block is shorter than the boundary peak, the difference is added to the total water units.
4. **Movement**: We move the pointer from the shorter side inward until the two pointers meet.
  
## Tech Stack & Implementation

**HTML5/CSS3**: Used to build the layout and style the block/water colors (Yellow for blocks, Blue for water).
**Vanilla JavaScript**: Handles the core algorithmic logic without external frameworks.
**SVG (Scalable Vector Graphics)**: Preferred method used to render the visual representation of the tank and the trapped water dynamically.

## Installation & Usage

1. Clone this repository.
2. Open the `index.html` file in any modern web browser.
3. Enter a set of block heights (comma-separated) in the input field.
4. Click **"Calculate"** to see the total units and the SVG visualization.

## Example Test Case

**Input**: `0,4,0,0,0,6,0,6,4,0`.
**Result**: `18 Units`.

