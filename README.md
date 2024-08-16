# ncurses_dinorunner

A C++ implementation of the Chrome dino game using ncurses for terminal display.

## Prerequisites

- C++ compiler
- CMake
- Conan 2

## Setup

1. Install Conan 2 if not already installed:
   ```
   pip install conan
   ```

2. Build and run:
   ```
   mkdir build && cd build
   conan install .. --output-folder=. --build=missing
   cmake .. -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Release
   cmake --build .
   ./dinorunner
   ```

## How to Play

- Press the spacebar to make the dino jump.
- Avoid the obstacles by jumping over them.
- The game ends when the dino collides with an obstacle.