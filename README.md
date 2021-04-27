# Tetris-Improved
Tetris with Classic and Modern Tetris Physics (Python)
Uses a freeCodeCamp Tetris template from the video https://youtu.be/zfvxp7PgQ6c

The purpose is to create a program that can play both the original early versions of NTSC Tetris (NES Tetris, Gameboy Tetris), as well as Modern tetris (most tetris games after 2006).  

=====================================================================

Classic Tetris Rules:
  - Piece generation is random, with one re-roll to try and combat repetition (yet, it isn't very good, as shown in this video of an 83 piece drought before spawning an "I" piece: https://youtu.be/1hIlqkwUcy0)
  - I did carry over hard drop from Modern Tetris by pressing up, and kept the ghost piece that shows where the piece will drop, even though these aren't in the original games.  However, I decided to keep the ghost piece that shows where the piece will drop, even if it is not in the original.
  - There is no piece rotation correction, also known as wall kicks.  If a piece cannot rotate, there is no correction to rotate it anyway.  (For example, try having a long bar on the right-most x coordinate.  If you try rotating, it will not work.)
  - There is an animation for clearing lines in an attempt to match the piece clear timing

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
