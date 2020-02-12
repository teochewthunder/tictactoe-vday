# Tic-tac-toe Valentine's Day Edition
This is a more intelligent version of the previous [Tic-tac-toe](https://github.com/teochewthunder/tictactoe) code. Normally, I would simply make another branch, but since this is new functionality rather than a "patch", a new repository seems more appropriate.

## CSS and Flavor Text
These are not really essential upgrades, but fun to have for the Valentines Day theme.

## Intelligence
This comes in the form of more checks. Initially, when the computer takes its turn, it simply places its marker on a random unclaimed square on the board. Now, the priosirites have shifted.

### Firstl Priority: WIN
Now, it checks through the *winPatterns* array for win conditions where a taken turn would immediately win the game.

### Second Priority: STOP YOU FROM WINNING
If no win condition exists, it checks for a win condition for *you*, and places its marker there to "block".

### Last Priority
If the above is *false*, then it randomly chooses a square to play.

*Note: Again, this does not work on Internet Explorer and Safari*
