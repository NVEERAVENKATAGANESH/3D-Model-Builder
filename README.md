veera venkata Ganesh Nurukurthi (G01448473)
# Model Builder - CS 663 Project 1
## Files
- main.cpp: The entry point of the application that sets up the GUI and handles rendering.
- tgaClass.cpp: Contains methods for loading and processing .tga images.
- tgaClass.h: The header file that defines the tgaClass class and its methods.
# Prerequisites
- Xcode Command Line Tools: To compile and build the program.
- FLTK library: Required for the GUI in this project.
- OpenGL: Pre-installed on macOS

# Install FLTK via Homebrew
If you haven't installed Homebrew:
 ' /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
'

- ** Then, install FLTK: **
' brew install fltk'

# Build Instructions

 - ** Navigate to the directory where the project files are **

 ** Compile the Project: ** 
 Use g++ to compile the project from the command line with the necessary OpenGL and FLTK flags:

 ' g++ main.cpp tgaClass.cpp -o ModelBuilder -framework OpenGL -framework GLUT -lfltk -std=c++11'

 ** Run the Application: Once compiled, run the program: **
  ' ./ModelBuilder'

# Usage
- Loading Images: The tgaClass file allows you to load .tga images, which can be used in the OpenGL rendering pipeline.
- Rendering: The main application is responsible for rendering the 3D model or other graphical elements using OpenGL.