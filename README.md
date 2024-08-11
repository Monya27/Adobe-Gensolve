Adobe GenSolve Hackathon

Project Overview

Curvetopia: A Journey into the World of Curves

Welcome to Curvetopia, where our goal is to bring order and beauty to the world of 2D curves! This project is an exploration into identifying, regularizing, and beautifying various types of curves. We focus on closed curves and progressively work with more complex shapes, covering symmetry and curve completion techniques.

Problem Statement

The objective of this project is to develop an end-to-end process that converts a PNG (raster) image of line art into a set of curves, where the curves are defined as a connected sequence of cubic Bézier curves. For simplification, instead of using PNG images as input, the project uses line art in the form of polylines, defined as a sequence of points.

Task Breakdown:
Regularize Curves:
Identify and regularize shapes such as straight lines, circles, ellipses, rectangles, rounded rectangles, regular polygons, and star shapes.
Test the algorithm with different images containing various shapes and verify the results.
Exploring Symmetry in Curves:
Identify symmetry in closed shapes, starting with reflection symmetry.
Transform the presentation as a set of points to identify and fit identical Bézier curves on points that are symmetric.
Completing Incomplete Curves:
Create algorithms using computer vision techniques to identify and naturally complete incomplete 2D curves that have gaps due to occlusion removal.
Code Explanation

Main Functions
read_csv(csv_path): Reads a CSV file containing paths of points defining polylines and returns a structured list of these paths.
create_precise_shape(shape_name, contour): Generates precise geometric shapes (e.g., circle, rectangle, star) based on the identified contour.
identify_shape(contour): Identifies the shape of the contour based on the number of vertices and other geometric properties.
refine_contour(contour): Refines the contour for better shape approximation.
regularize_shapes(path_XYs): Regularizes the shapes by identifying and refining the contours, then creating precise geometric shapes.
plot_shapes(regularized_shapes): Plots the regularized shapes for visualization.
write_output_csv(regularized_shapes, output_csv_path): Writes the regularized shapes to a new CSV file.
