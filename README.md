TicTacToe
=========

A single player tictactoe game in which it's impossible for the human to defeat the computer. 
The computer player was programmed using 2 different methods: rule based and minimax

Rule Based TicTacToe game (rules.html)

The Rule Based TicTacToe game uses a set of rules which the AI follows to play a move. The rules can be summed up as:

1. Either play in centre of the board or on the top left corner for the first computer move.
2. Try and win the game if you have the chance (make three in a row)
3. If the opponent has a chance to win, try and block his victory
4. If the human starts the game, play the second computer move directly below the first 'X' you come across 
   (assuming the human player is 'X'). This prevents any forks etc.
5. If the computer has to make a move which does not fall under any of the rules above, just play randomly in an empty space.

These rules may not be the ideal strategy for the computer to win a game. But it makes the computer impossible to beat.
The first 3 rules are fairly intuitive for a person who has played a lot of TicTacToe. Rule number four took me a while to figure
out, but it works! It's an easy way for the computer to avoid and create forks.

Minimax TicTacToe game (minimax.html)

Minimax is a standard strategy used by computers in a number of board games. The details how it works can be read on 
http://en.wikipedia.org/wiki/Minimax

To summarize minimax works in a way to maximize the gain and minimising the loss while playing a move. It extrapolates possible
endings, and chooses the best move from the options presented to the computer. Minimax itself is not the ideal strategy as it 
has certain drawbacks (not discussing these), but it's close the ideal. 

Rule Based vs Minimax

Comparing the two implementations, there are key advantages and disadvantages to using each one. The rule based strategy is much
quicker than minimax. It uses much less processing power and is perhaps ideal for a standard 3X3 game tictactoe game. It's main
drawbacks are that it is not extendable to larger boards, different rules, and perhaps not the best strategy to actually win a 
game. The minimax implementation scores on these fronts.
