# Xonic Game (XonicGamePF)

Professional, minimal README for the XonicGamePF project — a small 2D C++ game built with SFML.

## Table of contents
- Project
- Features
- Repository layout
- Requirements
- Build & run
- Contributing
- License

## Project

Xonic is a compact 2D game implemented in C++ using the SFML library. This repository contains the game source, assets, and helper files to compile and run locally inside a Linux development environment or container.

## Features

- Simple 2D gameplay with sprite-based graphics
- Audio support and basic score keeping
- Easy-to-read C++ source for learning and modification

## Repository layout

- Xsonic/: Game source and assets
  - main.cpp — main entry point
  - correct.cpp — game logic helper (compile together)
  - compile.txt — example compile commands
  - audio/, fonts/, images/ — asset folders
- scores.txt — persistent score storage
- README.md — this file

## Requirements

- Linux (development container provided)
- C++ compiler with C++17 support (g++ or clang++)
- SFML (Simple and Fast Multimedia Library)
  - Debian/Ubuntu: `sudo apt install libsfml-dev`

## Build & run

Quick compile (example):

1. Install SFML if missing:

	sudo apt update
	sudo apt install build-essential libsfml-dev

2. Compile (from repository root):

	g++ -std=c++17 Xsonic/main.cpp Xsonic/correct.cpp -o xonic -lsfml-graphics -lsfml-window -lsfml-system -pthread

3. Run the game:

	./xonic

Notes:
- If compilation flags or source files differ, consult `Xsonic/compile.txt` for examples.
- Run from the repo root so asset relative paths in `Xsonic/` resolve correctly.

## Contributing

Contributions are welcome. Suggested workflow:

1. Fork the repository and create a feature branch.
2. Make changes and add clear commit messages.
3. Open a pull request describing your changes.

Please ensure builds succeed and include any relevant test steps.

## License

This project is provided under the MIT license. See LICENSE or add one if required.
