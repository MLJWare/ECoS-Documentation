# Introduction to ECoS

ECoS is a modern fantasy console with a solid Entity-Component-System
 at its backbone, made by Mikkel Lykke Jørgensen (aka MLJWare) for the 
Fantasy Console Development Jam 2017.

ECoS is a modern fantasy console based around the solid foundation of
 an Entity-Component-System architecture (ECS). Once learned, the use of
 an ECS can make game development and prototyping much faster and keep 
your code much more modular, making it easy to reuse, alter and extend 
any part of your games.

To further enhance this modularity, ECoS allows for splitting your 
game code into multiple files, using the special 'USE' function to load 
them into other files (see "API-ECoS.txt" in the downloads).

ECoS features a full game development stack, including an image 
editor for drawing the game sprites, a synthesizer/tracker for making 
sound effects and music, a basic level editor for designing the game 
level, and a text editor for writing the game code.

## ​Specs

ECoS runs a 60 FPS, with a 128 by 128 resolution 1-bit display (5x 
scale); a limit of 255 sprites of 4 by 8 pixels, each with an additional
 8 bits for flags; 1 level/map of 256 by 32 tiles (each tile consisting 
of to consecutive sprites); a limit of 64 sound effects/melodies of 64 
nodes, each using one of 5 waveforms; the ability to build games into 
single file cartridges that include all the resources and files for the 
game to run; and the ability to mount cartridges from a file into 
memory.

## Modes/Editors

ECoS currently has seven different modes/editors:
* A Terminal/Command Prompt for general accessibility.
* A Text/Code Editor for writing game code.
* A Sprite/Tile Editor for drawing the game art.
* A Level/Map Editor for building the game world.
* A Tracker/Sequencer for creating the game music.
* A Synthesizer/Waveform Editor for making sound effects.
* A Game Mode for running the games.

## Programming

Games in ECoS are written as regular Lua 5.1 code, but without th 
standard libraries. Instead, ECoS provides a custom set of values and 
funtions, specifically for making games for the ECoS console.

## Getting Started

* [Tutorial: Snake](./tutorial/Snake.html)