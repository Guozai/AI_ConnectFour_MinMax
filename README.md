# AI_ConnectFour_MinMax
A python program to play Connect Four with people

Since the winning patterns are limited, I listed them out according to each piece. For instance, for piece (5,0), which is the position of the bottom left corner, all ‘possible 4 in rows’ is listed as below:
[ ][ ][ ][ ][ ][ ][ ]
[ ][ ][ ][ ][ ][ ][ ]
[X][ ][ ][X][ ][ ][ ]
[X][ ][X][ ][ ][ ][ ]
[X][X][ ][ ][ ][ ][ ]
[X][X][X][X][ ][ ][ ]
Unfortunately, I set the row 0-5 different from the board settings. So my row 0 is the row 5 of the board, which is the bottom row. These ‘4 in rows’ are saved into a nested dictionary with each row number (5 - board.row) as the outer index and each column number as the inner index. The value of each column key is a list of (row, col) pairs.

Ref:
Martin Saveski 2009, AI Agent for Connect Four, http://web.media.mit.edu/~msaveski/projects/2009_connect-four.html
