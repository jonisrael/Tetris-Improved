# Tetris-Improved
Tetris with Classic and Modern Tetris Physics (Python)
Uses a freeCodeCamp Tetris template from the video https://youtu.be/zfvxp7PgQ6c


Critical Bug Fixes:
- Fixed a line clear calculation bug when clearing three or four lines with non-cleared line(s) in-between.
- Fixed having pieces hang off the top of the grid, leading to accidental game-overs.
- Fixed game-over rule to match regular tetris, where the game ends if a piece cannot spawn, instead of if a piece goes above the grid
- Changed function of down key to drop one cell, then shortly after, alter gravity to dropping 30 cells per second until key is no longer pressed. 


Quality of Life Changes:
- Added Pause Function
- Added tutorial

Global Changes to both Classic and Modern tetris:
- Changed controls
- 

Classic Tetris attempts to emulate NES and Gameboy Tetris as close to original as possible.  Changes I included were:
- Added a DAS key repeat
