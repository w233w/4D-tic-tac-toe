# 4D tic tac toe

## Introduction

This game is an advanced version of tic tac toe. You can find the rules on Game Play section. \
Game development from pygame.

## Start Game
```shell
$python 4d_tic_tac_toe.py
```

## Game Play

### !Read First!

**Currently the start game screen is blank, you have to click mouse anywhere on blank screen once to start the game.**

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

The game will be held on a 3*3 tic-tac-toe chessboard. \
The first move has to be played on the middle chessboard.
The grid you played on the chessboard will determine the next chessboard you can play, a red border will help you where it is. \
eg. Player one plays on [2, 2] on a chessboard, next player must play on [2, 2] chessboard over the whole game board except the special case. \
On the chessboard, if any player has 3 of the same marks in a row, the player will own the chessboard, and the chessboard will lock. If the chessboard finished without a winner, the chessboard will be locked without an owner. \
The special case: If the next chessboard one player has to play to is locked, that player gains "free play" which means can play anywhere. \
The locked chessboard becomes inactive. \
The player who owns the chessboard 3 in a row win.

## TODO

1. Simple UI let player click info buttom to read the game rule --Maybe put the rule on start screen
2. Simple UI let player can see who will play next

## Known Bugs

* Locked chessboard also show the border and can't be removed. 
