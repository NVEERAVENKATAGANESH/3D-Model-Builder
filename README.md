OpenGL Robot Model Animation

This project demonstrates a 3D robot model built and animated using OpenGL and GLUT in C++. The application renders a robot composed of primitive 3D shapes and provides interactive controls for camera rotation, zooming, and animation speed.

The project also includes a custom TGA image loader for handling .tga textures used in OpenGL rendering.

Features

Interactive 3D robot model rendering

Robot constructed using OpenGL primitives:

Cubes

Spheres

Cylinders

Cones

Animated robot movement

Moving arms and legs

Facial animation (eyebrows and expressions)

Body movement animation

Mouse-based camera control

Rotate the scene using a trackball-style interaction

Context menu controls

Start / Stop animation

Zoom in / Zoom out

Increase / decrease animation speed

Reset the scene

Custom TGA image loader

Supports 24-bit and 32-bit TGA images

Validates image dimensions and formats

Project Structure
OpenGLApp/
│
├── main.cpp        # Main application file responsible for rendering and animation
├── tgaClass.cpp    # Implementation of the TGA image loader
├── tgaClass.h      # Header file defining the TGA loader class
└── README.md       # Project documentation
Technologies Used

C++

OpenGL

GLUT

FLTK

macOS Xcode Command Line Tools

Prerequisites

Before building the project, install the following dependencies.

Install Xcode Command Line Tools:

xcode-select --install

Install Homebrew (if not installed):

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Install FLTK:

brew install fltk

OpenGL and GLUT are already included with macOS.

Build Instructions

Navigate to the project directory and compile using g++:

g++ main.cpp tgaClass.cpp -o ModelBuilder -framework OpenGL -framework GLUT -lfltk -std=c++11
Run the Application
./ModelBuilder

This launches the OpenGL window displaying the animated robot.

Controls

Mouse Controls

Left Mouse Drag
Rotate the camera around the robot.

Keyboard Controls

Q — Quit the program
ESC — Exit the application

Right Click Menu

Right-click in the window to access the control menu.

Menu options include:

Start Animation

Stop Animation

Zoom In

Zoom Out

Speed Up

Slow Down

Reset Scene

Quit

Learning Objectives

This project demonstrates key concepts in computer graphics, including:

3D transformations and hierarchical modeling

Lighting and materials in OpenGL

Animation using transformation updates

Event-driven interaction with GLUT

Custom texture loading using TGA images
