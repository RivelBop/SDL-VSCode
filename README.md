# SDL-VSCode
A sample SDL3 starter project for VS Code (may even work for CLion).

## Getting Started
### C++ Environment (Windows)
1. [Compiler](https://code.visualstudio.com/docs/cpp/config-mingw)
2. [CMake](https://cmake.org/download/)
3. [Ninja](https://github.com/ninja-build/ninja/wiki/Pre-built-Ninja-packages#windows)
4. [VS Code](https://code.visualstudio.com/Download)
5. [C++ VS Code Pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools-extension-pack)

### C++ Environment (MacOS)
1. [Compiler/Clang/XCode](https://apps.apple.com/us/app/xcode/id497799835?mt=12/)
2. [CMake](https://cmake.org/download/)
3. [Ninja](https://github.com/ninja-build/ninja/wiki/Pre-built-Ninja-packages#mac)
4. [VS Code](https://code.visualstudio.com/Download)
5. [C++ VS Code Pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools-extension-pack)

### Installing SDL3
[SDL3 Setup Guide](https://github.com/libsdl-org/SDL/blob/main/INSTALL.md)  
[SDL3 Setup CMake](https://github.com/libsdl-org/SDL/blob/main/docs/INTRO-cmake.md)

In Command Line:  
`git clone https://github.com/libsdl-org/SDL.git vendored/SDL`  
`git clone https://github.com/libsdl-org/SDL_image.git vendored/SDL_image`  

Look into home directory, copy vendored folder into project source folder.

### Exporting and Releasing (Windows)
1. `cmake -S . -B build/release -G "Ninja" -DCMAKE_BUILD_TYPE=Release`
2. `cmake --build build/release`

### Exporting and Releasing (MacOS)
Look inside of `CMakeLists.txt` and `build.sh` for commented changes.
