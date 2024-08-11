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


## Isolated Output
![WhatsApp Image 2024-08-11 at 22 46 42](https://github.com/user-attachments/assets/64006328-42fb-49c1-b784-439393d2d4b0)
## Occlusion Output
![occlusion1](https://github.com/user-attachments/assets/a235e3ce-d658-415e-bb9b-2f6da531c914)
## Occlusion Output
![occlusion2](https://github.com/user-attachments/assets/59d947da-ff57-4acc-a353-64694df97efa)
