# Cplusplus-program-cs330
# CS 330 Computational Graphics and Visualization

## Project Overview

For this project, I developed an interactive 3D desktop scene using C++, OpenGL, and Visual Studio. The scene includes a laptop, desk, pencil holder, pencil, notebook, and desk lamp. I used primitive shapes, textures, lighting, and camera controls to create a recognizable workspace.

This repository contains the 3D Scene ZIP folder and Design Decisions document.

## How do I approach designing software?

I approach software design by breaking a larger problem into smaller parts. For this project, I identified the basic shapes that could represent each object before focusing on its details. Boxes formed the laptop and notebook, cylinders formed the pencil holder and lamp supports, and cones formed the pencil tip and lamp shade.

The project helped me develop skills in spatial planning, object composition, and visual consistency. I learned how scaling, rotation, and translation work together to position objects. I also learned to consider textures and lighting as part of the design because they affect how clearly users can recognize the objects.

My design process followed the course milestones. I started with basic geometry, added camera interaction, applied textures, and then refined the lighting and overall scene. In future projects, I can use this same approach: establish the core structure first, then add detail and evaluate the result against the requirements.

## How do I approach developing programs?

I develop programs by building and testing manageable pieces of functionality. In this project, I reused drawing helpers and transformation functions instead of repeating the same OpenGL operations for every component. Separating scene construction from camera management also made the code easier to understand and change.

Iteration was essential. I repeatedly built the application, inspected the scene, and adjusted object placement, materials, and lighting. For example, I corrected a diagonal lighting seam by removing a normal reversal in the fragment shader. I also changed the projection controls so switching between perspective and orthographic views preserved the camera’s position and orientation.

Throughout the milestones, my approach shifted from getting individual objects to appear to making the complete application consistent and maintainable. I paid more attention to reusable functions, predictable controls, file paths, and packaging. Moving the project also showed me why testing outside the original working folder matters: source code alone is not enough when the application depends on shared libraries, shaders, and textures.

## How can computer science help me reach my goals?

Computer science helps me turn ideas into working applications through problem solving, logical reasoning, and testing. This project strengthened my understanding of how mathematics and programming work together to produce an interactive visual result.

For my future education, computational graphics provides a foundation for studying transformations, coordinate systems, rendering, and user interaction. These concepts also connect to other subjects, including simulation, interface design, and data visualization.

For my professional development, the project gave me practice organizing a C++ application, debugging problems across multiple files, and explaining technical decisions. Those skills apply beyond graphics programming. Whether I work on visualization tools, interactive applications, or other software, I can use the same habits of modular development, incremental testing, and clear documentation.

## Camera Controls

- W / S: Move forward and backward
- A / D: Move left and right
- Q / E: Move upward and downward
- Mouse: Change viewing direction
- Mouse wheel: Adjust movement speed
- O: Switch to orthographic projection
- P: Switch to perspective projection
- Escape: Close the application

## Building the Project

Extract the complete project ZIP before opening the solution in Visual Studio. Keep the Projects, Libraries, Utilities, and 3DShapes folders together so the relative dependency paths remain valid.

Open the solution inside Projects/7-1_FinalProjectMilestones, select the x86/Win32 configuration, and build the solution. Run the scene from Visual Studio so its textures and shaders load from the expected working directory.
