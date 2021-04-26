# Tetris-Improved
Tetris with Classic and Modern Tetris Physics (Python)
Uses a freeCodeCamp Tetris template from the video https://youtu.be/zfvxp7PgQ6c

The purpose is to create a program that can play both the original early versions of NTSC Tetris (NES Tetris, Gameboy Tetris), as well as Modern tetris (most tetris games after 2006).  In general, classic Tetris has a almost completely randomized piece system, while later tetris games have 7 piece random bags, which means that there is a guarantee that certain pieces will be generated within 1 to 13 pieces.

Critical Bug Fixes:
  - Fixed a line clear calculation bug when clearing three or four lines with non-cleared line(s) in-between.
  - Fixed having pieces hang off the top of the grid, leading to accidental game-overs.
  - Fixed game-over rule to match regular tetris, where the game ends if a piece cannot spawn, instead of if a piece goes above the grid
  - Fixed bug where pieces were sometimes locked in mid-air
  - Changed function of down key to drop one cell, then shortly after, alter gravity to dropping 30 grid-cells per second until key is no longer pressed.
  - Added error handler to pause before a potential crash


Quality of Life and Global Changes:
  - Added counterclockwise rotation
  - Added a ghost piece (location where the piece will drop)
  - Added Pause Function
  - Added Tutorial and changed keys to be more ergonomic
  - Added Mode and Level functions
  - Added Score, Lines, Level, and Tetris rate on in-game UI
  - Added a 3-2-1-Go function at the beginning
  - Changed how pressing and holding the down key worked to match other tetris games
  - Added Delayed Auto Repeat.  Classic Tetris is about 10 grid-cells per second with , Modern tetris is about 30 per second

Classic Tetris Changes
  - Added counterclockwise rotation (Global)
  - Changed how pressing and holding the down key worked (Global)
  - 
  - Added hard-drop function by pressing up (Modern Only)
  - Changed controls to be more ergonomic
  - Added

Global Changes to both Classic and Modern tetris:
- Added 
- 

Classic Tetris attempts to emulate NES and Gameboy Tetris as close to original as possible.  Changes I included were:
- Added a DAS key repeat
