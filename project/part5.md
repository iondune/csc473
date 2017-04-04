---
layout: page
permalink: /project/part5/
title: "Program 5 - Spatial Data Structures"
---

Due Thursday May 26th, at 11:55pm

---

## Goals for assignment 5:

For this portion of your ray tracer, your program needs to:

- compute intersections and appropriate shading for boxes
- handle large files (e.g. balls.pov and bunny.pov) in reasonable times by including either a bounding volume hierarchy (BVH), binary space partitioning tree (BSP tree) or an oct-tree (ie a spatial data structure) in your code to optimize ray intersection testing

Example files and results will be posted and announced on email.
You will need to create your own visually interesting scene that you render and submit the .pov file.

---

## What you should hand in via polylearn:

- Your code, include all files necessary to compile and run your ray tracer, including a Makefile or cmakeLists.txt
- A README.txt file with any information about what is working or not working with your implementation to assist the grader in determining what is causing potential errors in your output and help in assigning partial credit.
- Your own .pov file and rendered image of an interesting scene

You need to handin your code and images generated using poly learn.
Look for the assignment directory.

## Grading breakdown:

- 25 spatial data structure
- 15 points working box intersections
- 10  general sanity

---

To get full credit for your spatial data structure - your code just has to be as fast or faster then my very old code with still many printfs:

times are:

- gnarly: `44` seconds
- balls2: `31` seconds

Image size is 640 x 480 and I did *not* have anti-aliasing in place for those timings.

Don't worry if you are slower then these, you can still get credit for your spatial data structure, if you can show that your raytracer performance is enhanced by at least 20% using a spatial data structure.

---

Program execution – same as before:
Your program should have the following syntax:
  `raytrace <width> <height> <input_filename> <BRDF>`

Sample input files and images are given on the class webpage.
Some of these pictures may be generated by Povray and will not look identical to your output (due to differences in the shading model, etc.).