# Pong Game in x86 Assembly

This repository contains a classic Pong game implemented in x86 assembly language for the DOS environment. The game runs in VGA text mode and demonstrates key concepts of low-level programming, including direct memory manipulation, game logic, and collision handling.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [How to Run](#how-to-run)
- [Controls](#controls)
- [Gameplay](#gameplay)
- [Files](#files)
- [Roadmap](#roadmap)
- [Contributing](#contributing)

## Features

- **Game Elements**: 
  - Ball and two paddles.
  - Scoring system with a winning condition.
  
- **Rendering**:
  - Direct manipulation of VGA text memory to render the game board, paddles, and ball.
  
- **Paddle Controls**:
  - Player 1 and Player 2 paddles can move up, down, left, and right.

- **Score Display**:
  - Real-time score updates.
  - Victory message when a player reaches the winning score.

## Prerequisites

- **Environment**: The game is designed to run in a DOS environment. Use an emulator like [DOSBox](https://www.dosbox.com/) or download it from [SourceForge](https://sourceforge.net/projects/dosbox/) for modern systems.
- **Assembler**: The project uses NASM for assembling the code. A beginner-friendly guide (`AFD_Tutorial.pdf`) is provided for reference.

## How to Run

1. **Install DOSBox**:
   - Download and install DOSBox from one of the following links:
     - [Official DOSBox](https://www.dosbox.com/)
     - [DOSBox on SourceForge](https://sourceforge.net/projects/dosbox/)
   
2. **Set up NASM**:
   - Unzip the provided `nasm.zip` file into a directory of your choice.

3. **Copy Source File**:
   - Place the `pingpong.asm` file into the extracted NASM folder.

4. **Launch DOSBox**:
   - Open DOSBox and mount the NASM directory:
     ```bash
     mount a: <path_to_nasm_directory>
     a:
     ```

5. **Assemble the Code**:
   - Assemble the Pong game using NASM:
     ```bash
     nasm pingpong.asm -o pingpong.com
     ```

6. **Run the Game**:
   - Start the game:
     ```bash
     pingpong.com
     ```

## Controls

- **Player 1 (Paddle 1)**:
  - Move Up: UP KEY
  - Move Down: DOWN KEY
  - Move Left: LEFT KEY
  - Move Right: RIGHT KEY

- **Player 2 (Paddle 2)**:
  - Move Up: W
  - Move Down: S
  - Move Left: A
  - Move Right: D

## Gameplay

- The first player to score 5 points wins.
- The game displays a victory message for the winning player.

## Files

- `pingpong.asm`: The main assembly source code for the game.
- `DOSBOX.zip`: Includes the DOSBox emulator for running the game.
- `AFD_Tutorial.pdf`: A tutorial for setting up the NASM assembler.

## Roadmap

- Add ball movement logic.
- Implement collision detection for paddles and walls.
- Include sound effects for scoring and collisions.
- Enhance visuals with color.

## Contributing

Contributions are welcome! Feel free to fork this repository, make improvements, and create a pull request.

Feel free to suggest improvements or report issues in the [Issues](https://github.com/yourusername/pong-assembly/issues) section.
