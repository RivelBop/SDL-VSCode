# SDL-VSCode
A sample SDL3 starter project for VS Code (may even work for CLion).

## Getting Started
### Installing SDL3
[SDL3 Setup Guide](https://github.com/libsdl-org/SDL/blob/main/INSTALL.md)  

In Command Line:  
`git clone https://github.com/libsdl-org/SDL.git vendored/SDL`  
`git clone https://github.com/libsdl-org/SDL_image.git vendored/SDL_image`  

Look into home directory, copy vendored folder into project source folder.

### Exporting and Releasing (Windows)
1. `cmake -S . -B build/release -G "Ninja" -DCMAKE_BUILD_TYPE=Release`
2. `cmake --build build/release`

### Exporting and Releasing (MacOS)
Look inside of `CMakeLists.txt` and `build.sh` for commented changes.
