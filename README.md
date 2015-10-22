# Stephen's Game of Life
This is an implementation of John Conway's cellular automaton "Game of Life" with added features

### How to play:
It's a zero-player game, but you can determine the rules! The game is a continuous view of new generations of cells, whose lives are represented by colored cells on the grid. A white cell is dead and has never been alive. A fully colored cell is a living one. A faded cell is dead, but it has been alive before. Here's how you control the rules:

1. Width/Height: Enter numbers between 20 and 200 to control the dimensions of the grid
2. Radius: Enter a number between 1 and 10 to control how far a cell's neighbors extend. "1" indicates that a cell should only consider its immediate (8) neighbors. "2" indicates that a cell will consider the next shell (total 16), and so on.
3. LThresh: This is the loneliness threshold that determines the number of neighbors below which a cell will die as if by underpopulation. This number should be greater than 0 and no more than the overpopulation threshold.
4. OThresh: This is the overpopulation threshold that determines the number of neighbors above which a cell will die. This number should be at least the loneliness threshold and no greater than one less than the total number of neighbors for any given cell.
5. GenMin: This is the minimum number of neighbors above which a dead cell will generate. This number should be greater than 0 and no more than GenMax.
6. GenMax: This is the maximum number of neighbors below which a dead cell will generate. This number should be at least GenMin and no greater than one less the total number of neighbors for any given cell.
7. Edge Neighbor Behavior: This determines how cells behave at the edges of the world.
  * A cell will consider off-grid neighbors to be alive if "All Alive" is selected.
  * A cell will consider off-grid neighbors to be dead if "All Dead" is selected.
  * A cell will wrap to the corresponding opposite side if "Toroidal" is selected.

View here: http://htmlpreview.github.io/?https://github.com/sjyan/game-of-life/blob/master/conway.html
