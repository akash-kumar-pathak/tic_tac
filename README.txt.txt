# tic_tac
-Components
Now let's talk about the TicTacToe element. Players will compete inside 3x3 cell squares that will serve as our game board. We'll use a multi-dimensional array to specify our board: Now let's talk about the TicTacToe element. Players will compete inside 3x3 cell squares that will serve as our game board. We'll use a multi-dimensional array to specify our board.
From this array, we'll draw the board on the DOM. The first row and column contain the first cell, the second row and column contain the second cell, and the third row and third column contain the third cell. Up until the final cell, it continues in this way.

The next step is to build an object that will store each player's name and game-related symbol. We will be competing against the computer 

-Creating functions and Usestates:
The TicTacToe component is now created.
We make a useState Hook in order to hold the board. We’ll create additional Hooks to hold the turn and the winner

board state: Holds the multi-dimensional array of the board
setBoard function: Sets the board
isCPUNext state: Holds the turn of the player
setIsCPUNext function: Sets the turn
winner state: Holds the winner of the game
setWinner function: Sets the winner

We can see that we put the value into the first cell, giving us the first array in the board array and the first element in the array. The second cell received a similar treatment, and eventually all of the cells.
We also called the playFn function with the appropriate index of the array in the board and the index in that same array, enabling us to capture wherein the board we will place the symbol.
We’ll create the function playFn. When a user clicks on it, it will play the game.

The playFn function will check if the game is over. If it is, it will display the winner. If not, it will check if the player is next. If it is, it will set the player’s symbol to the particular index of the array in the board array and call the setBoard function to set the board state. Then, it will call the checkWinner function to check if the game is over. Finally, it will set isCPUNext to true.
The checkWinner function, which will determine if the game is over, will then be created. It will come back if it is. If not, it will determine whether the player or the CPU has triumphed. If the player has triumphed, the winning state will be changed to HUMAN. If the CPU has triumphed, the winner state will be changed to CPU. If there is a tie, the winner state will be set to draw. If there is no draw, it will go back to.










