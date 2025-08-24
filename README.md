# An assignment repository
This repository is a C++ workspace supported by a cross-platform Docker-based dev container. The header (`.h`) files should be placed under the `include/` folder, while the implementation (`.cpp`) files should be placed under the `src/` folder.

## Requirements

This repository requires the following one-time setup:

- Install the [Docker desktop application](https://www.docker.com/products/docker-desktop/). You don't need to do anything with Docker other than installing it on your operating system.
- Install [Visual Studio Code](https://code.visualstudio.com).
- Open Visual Studio Code and install the Dev Containers extension.

Having done that, download or clone this repository into your local machine and open its folder in Visual Studio Code. If you see a popup with an option to "Reopen in Container," click that. Otherwise, click on the Dev Containers icon at the bottom left corner and select "Reopen in Container." You can also type F1 to launch VSCode's Command Palette and search for and select "Dev Containers: Reopen in Container." This will reopen this repository in the dev container where all development environment tools (compiler, linker, debugger, etc.) are available.

## Build
Inside the assignment folder created by the command “git clone”, run the following commands:
```
cd build
cmake ..
```
You only need to run these commands once.

## Compile and test
From inside the build folder (run `cd build` if needed), run the following commands to compile and test your code:

```
make tester
./tester
```

Make sure all the test cases/assertions pass.

You may run a subset of the test cases by passing an argument tag.

```
./tester [tag1]
```

This will run all the test cases tagged with `[tag1]`.

## Compile and run
From inside the build folder (run `cd build` if needed), run the following commands to compile and run your application:

```
make main
./main   
``` 

**NOTE**: All files should be read from or written to the `resources` folder.
