# Adobe GenSolve Hackathon

## Project Overview

Curvetopia: A Journey into the World of Curves
Welcome to Curvetopia—where the elegance of mathematics meets the artistry of design. Our mission? To breathe life into 2D curves by identifying, regularizing, and enhancing them with precision and beauty. In this project, we dive deep into the world of closed curves, progressively tackling more complex shapes, symmetry, and curve completion techniques.

## Problem Statement

In a world dominated by pixels, creating smooth, scalable graphics requires more than just raster images. Our challenge is to develop a sophisticated process that transforms a PNG (raster) image of line art into a seamless set of curves. These curves are defined as a connected sequence of cubic Bézier curves, known for their versatility and smoothness in digital graphics. To simplify, we've chosen to work with line art in the form of polylines—sequences of points representing the essence of the shapes.

## Task Breakdown

### 1. Regularize Curves
Objective: Identify and standardize shapes, including straight lines, circles, ellipses, rectangles, rounded rectangles, regular polygons, and star shapes.
Approach: Test the algorithm with diverse images containing these shapes, ensuring accuracy and consistency.
### 2. Exploring Symmetry in Curves
Objective: Uncover and utilize symmetry in closed shapes, beginning with reflection symmetry.
Approach: Convert the presentation of points to fit identical Bézier curves on symmetric points, enhancing the regularity and aesthetic appeal of the shapes.
### 3. Completing Incomplete Curves
Objective: Develop algorithms to naturally complete 2D curves with gaps, a common issue due to occlusion or removal.
Approach: Leverage computer vision techniques to identify these gaps and propose the most natural curve completion.
Code Explanation

Here's a quick look at the key functions that power Curvetopia:

read_csv(csv_path): Reads the CSV file containing polyline paths and returns a structured list of these paths.
create_precise_shape(shape_name, contour): Generates precise geometric shapes (e.g., circles, rectangles, stars) based on the identified contours.
identify_shape(contour): Analyzes the contour to identify the shape by examining vertices and geometric properties.
refine_contour(contour): Refines contours to improve shape approximation.
regularize_shapes(path_XYs): Regularizes shapes by refining contours and generating precise geometric representations.
plot_shapes(regularized_shapes): Visualizes the regularized shapes, offering a clear view of the transformation.
write_output_csv(regularized_shapes, output_csv_path): Exports the regularized shapes to a new CSV file.
Execution

Input
File: A CSV file (/content/frag2.csv) containing polyline paths.
Processing
Action: The polyline paths are read, regularized, and visualized for analysis.
Output
File: The processed, regularized shapes are saved in a new CSV file (/content/frag2_output.csv), ready for further exploration or deployment.
