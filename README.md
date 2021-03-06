# Haskell Minesweeper

A version of the game Minesweeper written in the Haskell programming language.

The game can be played using the terminal or on a web browser using the ThreePenny-GUI.

It also comes with a computer solver which attempts several techniques to try to automatically solve the grid. It can make any obvious moves. If there are none available, it uses a modified version of the Tank solver algorithm (https://luckytoilet.wordpress.com/2012/12/23/2125/). If it can't find any safe moves, it attempts to work out the probability that each square is a mine and picks the one which is least likely to be a mine. Unfortunately, it is unable to work out the true probability as this would be very complicated however, it can still make a good guess. Its results when playing with the following difficulties is reported below.

| Tables        | Won        | Played  | Percentage   |
| ------------- |------------|---------| ------------ |
| Beginner      | 17         |    20   |  85%         |
| Intermediate  | 11         |    20   |  55%         |
| Expert        | 1          |    20   |  5%          |
