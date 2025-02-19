# Interactive Measurement Dashboard

## Overview

Your task is the create an interactive measurement dashboard React and TypeScript, where users can draw two rectangles on a canvas, calculate the dimensions and distance, and save these details to a table stored in local storage.
Clicking a record in the table should re-render the shapes in their original positions on the canvas.

## Requirements

1. Interactive Canvas.
  - Allow users to draw two rectangles on the canvas
  - Rectangles are drawn by clicking and dragging.
  - Once rectangles are drawn, display their dimensions. And distance between their centers.
  - Prevent drawing more than two rectangles at a time. Users should clear the canvas or save the data before drawing more.

2. Save Functionality.
  - After drawing two rectangles, users can click a "save" button to store rectangle data in local storage.
  - Clear the canvas after saving.

3. Measurement data table.
  - Display a table showing all saved records, each row should display:
    ```
    i. Rectangle 1 dimensions
    ii. Rectangle 2 dimensions
    iii. Distance between rectangles
    iv. Timestamp when record was saved
  - Fetch data from local storage to populate the table when the app loads

4. Re-render on click.
  - Clicking on a row in the table should redraw the two rectangles on the canvas in their saved positions
  - Highlight the selected row in the table for better UX

5. Responsiveness.
  - Ensure the app is responsive and works well on both desktop and mobile
  - Use basic styling to make the layout clean and intuitive

## Bonus (Optional)

1. A React + TypeScript application with:
  - A working canvas for drawing two rectangles
  - Functionality to calculate rectangle dimensions and distance
  - Table integration with local storage for saving and retrieving data
  - Re-render functionality when clicking table rows

2. Submit the codebase with a README containing:
  - Assumptions or limitions
  - Steps to run the application