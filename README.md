# pygame_4d_tic_tac_toe

## Introduction

This game is an advanced version of tic tac toe. You can find the rules on Game Play section.

## Start Game
```shell
$python 4d_tic_tac_toe.py
```

## Game Play

### 中文

游戏在3*3的9个井字棋的棋盘上进行。\
第一手默认在[1, 1]处的井字棋的棋盘上落子。\
落子的位置决定了下一次落子的棋盘，同时红色边框也会提醒你可以落子的棋盘。\
例如：当玩家在棋盘上的[2, 2]处落子后，则下一手必须在[2, 2]处的棋盘上落子，除非出现例外。\
当某个棋盘上达成3连时，该棋盘被封锁并由3连的玩家持有。\
当一个棋盘9个格子被摆满而没有3连出现时，棋盘也会被封锁，并变成灰色。\
例外：当下一回合落子的位置是被封锁的棋盘时，下一回合的落子不再有棋盘限制。\
被封锁的棋盘不允许再落子。\
胜利的条件是持有的棋盘达成3连的玩家获胜。

### English

Game will be hold on a 3*3 tic tac toe chessboard. \
THe first ever play have to be played on middle chessboard. \
The grid you played on chessboard will determine the next chessboard you can play, a red border will help you where it is. \
eg. Player one play on [2, 2] in a chessboard, next player must play on [2, 2] chessboard over whole game board except the spcial case. \
When a chessboard finished, if any player has a 3 of kind on chessboard, the player will own the board. Other wise, chess boardlocked without owner. \
The special case: If next chessboard a player have to play is locked, that player gain a free play. \
Locked chessboard become inactive. \
The player who's owned chessboard achieve 3 of a kind win.

## TODO

1. Game logic to force player play on specific board or anyplace if on special case -- Done
2. Visual effect to let player know where they can play next -- Half Done, using a red border as notice.
3. Simple UI let player able to click (re)start -- Half Done, Blank start screen now.
4. Simple UI let player click info buttom to read the game rule --Maybe put the rule on start screen
5. Simple UI let player can see who will play next
6. Too many magical number, clear the code.

## Known Bugs

* Locked chessboard also show the border and can't be removed. 
* Click while fast mouse moving may cause unexpected error.
