# Tic-Tac-Toe-game
Sure! Let's go through the code line by line:

1. `def sum(a,b,c):` - This defines a function named `sum` that takes three parameters `a`, `b`, and `c`.

2. `return a+b+c` - This line inside the `sum` function returns the sum of the three parameters `a`, `b`, and `c`.

3. `def printBoard(xState,zState):` - This defines a function named `printBoard` that takes two parameters `xState` and `zState`.

4. The following lines within the `printBoard` function define variables `zero`, `one`, `two`, and so on, which represent the state of the Tic Tac Toe board. These variables are determined based on the values in `xState` and `zState` arrays, which represent the positions of 'X's and '0's on the board.

5. The `print` statements within the `printBoard` function display the Tic Tac Toe board using the values determined in the previous step.

6. `def checkwin(xState,zState):` - This defines a function named `checkwin` that takes two parameters `xState` and `zState`.

7. `wins=[[0,1,2],[3,4,5],[6,7,8],[0,3,6],[1,4,7],[2,5,8],[0,4,8],[2,4,6]]` - This line defines a list `wins` which contains lists representing all possible winning combinations in Tic Tac Toe.

8. The `for` loop in the `checkwin` function iterates over each possible winning combination.

9. Inside the loop, it checks if the sum of the values in `xState` corresponding to the current winning combination is equal to 3, indicating that 'X' has won. If so, it prints "X won the match" and returns 1.

10. Similarly, it checks if the sum of the values in `zState` corresponding to the current winning combination is equal to 3, indicating that '0' has won. If so, it prints "0 won the match" and returns 0.

11. If no player has won after checking all winning combinations, it returns -1.

12. `if __name__ =="__main__":` - This block checks if the script is being run as the main program.

13. `xState =[0,0,0,0,0,0,0,0,0]` and `zState =[0,0,0,0,0,0,0,0,0]` - These lines initialize the states of the board for 'X' and '0', respectively.

14. `turn = 1` - This initializes the variable `turn` to 1, indicating that it's 'X''s turn to play.

15. `print("Welcome to Tic Tac Toe")` - This line prints a welcome message.

16. The `while` loop runs indefinitely until the game is over.

17. Inside the loop, it prints the current state of the board using the `printBoard` function.

18. Depending on whose turn it is (`turn` variable), it prompts the user to input their move.

19. It then updates the state of the board accordingly.

20. It then calls the `checkwin` function to check if there's a winner. If there is, it prints "Match Over" and breaks out of the loop.

21. Finally, it toggles the turn between 'X' and '0' using `turn = 1 - turn`. This ensures that the turns alternate between 'X' and '0'.
