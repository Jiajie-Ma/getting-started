# getting-started
A simple demo to test whether GLFW, GLEW, OpenGL, and GLM are setup correctly

# Tools and dependencies

To obtain the source and generate build files, you will need to install git and cmake. To build, you will 
also need to install GLEW, GLFW, and GLM.

* GLEW: Needed for accessing openGL 4.0 features
* GLFW: Implements our window and user interaction events, such as mouse and keyboard 
* GLM: Implements useful vector and matrix functionality for graphics

On windows, the dependencies are included in this repository. For macOS, you will need to install them separately.

## Windows

On windows

* [Download and install git](git-scm.com/download/win).
* [Download and install cmake](https://github.com/Kitware/CMake/releases/download/v3.19.4/cmake-3.19.4-win64-x64.msi).

## macOS

On macOS, run the following commands in terminal

* `brew install cmake`
* `brew install glew`
* `brew install glfw3`

For GLM, you need to execute two commands

* `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" < /dev/null 2> /dev/null`
* `brew install glm`

# Build on windows

First, open the folder containing this source in Explorer. From here, right-click and open `Git Bash`. This will open a terminal window.

From git bash, run the following commands

* `mkdir build`
* `cd build`
* `cmake -G "Visual Studio 16 2019" ..`

The above commands will create Visual Studio project files inside the build folder. It is important to create the subdirectory `build`, to 
keep our repository clean of generated files. 

Double click on `CS312-GettingStarted.sln` to open the project. 
If you don't know where to start with visual studio, or need a refresher, [this video shows how to build, run, and debug with Visual Studio](https://youtu.be/hZ_ZZy0j7Vk)

# Build on macOS

From terminal, navigate to the folder containing this code. Then, run the following commands

* `mkdir build`
* `cd build`
* `cmake ..`
* `make`
* `./bin/testGLFW`

Running `cmake ..` will generate Makefiles for this project. Running `make` compiles the program. The last command runs the compiled program. You can also use Visual Studio to run and debug this program. It is important to create the subdirectory `build`, to 
keep our repository clean of generated files.

If you don't know where to start compiling and running C++, or need a refresher, [this video shows how to build, run, and debug with terminal or Visual Studio Code](https://youtu.be/DEytbPbfZVo)

