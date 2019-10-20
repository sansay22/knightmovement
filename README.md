# <center>The knight movements</centerThe>

### Task
In chess, the board is split in 8 rows and 8 columns. Considering the view of the game to be from the white side, the utmost top left cell is called a8 and the utmost top right cell is called h8. Decreasing from top to bottom of the chessboard, the utmost down left cell is then called a1 and the utmost down right cell is called h1.
Each position must be a valid chessboard-position notation (Algebraic notation) such that it is identified by a column identifier from a to h and a row identifier from 1 to 8.
Given a white knight and a set of chess pieces that can be yours (white) or not (black).
Print one of possible moves (if it’s possible) of knight for capture all opponent’s pieces in the current configuration.

## Input
First line: the position of the white knight
Second line: the amount P of pieces to be placed on the board
Next P lines: P space-separated lines containing attributes for each piece: color position

color is either 0 (WHITE) or 1 (BLACK)
position is the chessboard-notation of the position of the given piece.

Output
A list of space-separated combination where combination has the following shape:
K from_position, action, to_position with from_position being the actual position of the white knight and to_position being a possible destination for the white knight, both in the chessboard-position format. action should be x if the movement involves taking an opponent pieces, - otherwise.
For instance, if the white knight is in d5 and can move to d6, then the output must be Kd5-d6. If the white knight is in e4 and can capture an opponent piece in e3, then the output must be Ke4xe3.

Constraints
The grid is always an 8*8 matrix.


### Example

| Input  |  Output  |
| ------------ | ------------ |
|  f3 |  KF3-E5 |
| 2  |  KE5-D3 |
| 0 c1 | KD3xC1 |
|0 f2| KC1-D3|
| | KD3xF2|



