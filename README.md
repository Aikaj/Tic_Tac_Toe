# Tic_Tac_Toe
Fully class based tic tac toe game in python

Helper Functions::
1. display_board(board):

  Clears the current output and prints the current state of the Tic-Tac-Toe board.
  The board is represented by a list where the indices correspond to positions on the board:

7 | 8 | 9

---------

4 | 5 | 6

---------

1 | 2 | 3

2. player_input():
 Prompts Player 1 to choose either 'X' or 'O'.
 Returns a tuple containing Player 1's marker and Player 2's marker.

3. place_marker(board, marker, position):
 Places a player's marker ('X' or 'O') on the board at the specified position.

4.  win_check(board, mark):
 Checks if the given mark ('X' or 'O') has won the game by evaluating all possible winning combinations.

5. choose_first():
 Randomly decides which player goes first, returning 'Player 1' or 'Player 2'.

6. space_check(board, position):
 Checks if a given position on the board is free (i.e., not already occupied).

7. full_board_check(board):
 Checks if the board is completely filled. Returns True if the board is full, otherwise False.

8. player_choice(board):

 Prompts the current player to choose a position on the board.
 Ensures the chosen position is valid and not already occupied.

9. replay():

 Asks the players if they want to play again.
 Returns True if they choose 'Yes', otherwise False.

-- Main Game Loop

1. Initialization:

 Prints a welcome message.
 Enters an infinite loop to keep the game running until the players decide to stop.

2. Game Setup:

 Initializes an empty board (the_board = [' '] * 10).
 Prompts Player 1 to choose their marker, and assigns the markers to both players.
 Randomly decides which player goes first.
 Asks if the players are ready to start the game.

3. Game Play:

 Enters another loop that continues as long as game_on is True.
 Depending on whose turn it is:
 Displays the board.
 Prompts the current player to choose a position.
 Places the player's marker on the board.
 Checks if the current player has won or if the board is full.
 If there is a win or a tie, it sets game_on to False to end the game.
 Switches the turn to the other player.

4. Replay:

 After a game ends, asks the players if they want to play again.
 If the players choose 'No', breaks out of the main loop, ending the game.
 Code Example in Action

-- When you run this script, it will execute the following steps in sequence:

 Initialize the game.

 Prompt players to choose their markers.

 Randomly select which player goes first.

 Enter a loop to handle the game play.

 Continue looping, alternating turns between players, until a win or tie is detected.

 After the game ends, ask if the players want to play again.

 If 'Yes', restart the game; if 'No', exit the loop and end the script.

Improvements and Error Handling

 The current implementation assumes all user inputs are valid. In practice, you might want to add additional error handling for unexpected or invalid inputs     
 (e.g., non-integer inputs for positions, invalid characters for markers).
 The replay() function should ideally handle different cases of 'yes' and 'no' (e.g., case insensitive).
