# Tic_Tac_Toe_AI_Version

Problem Title:

Implement Tic Tac Toe Game with Minimax and Alpha-Beta Pruning Algorithm.

Problem Description:

In this assignment, we need to implement the classic game of Tic Tac Toe as an adversarial
search problem and develop an AI player using the minimax algorithm with alpha-beta pruning.
We have to create a program that allows human vs. computer and computer vs. computer
gameplay and should print the game board on the console after every move.

Tools and Languages Used:

➢ PyCharm IDE
➢ Python Language
➢ MS Word

Tik Tac Toe:

Tic Tac Toe is a game for two players on a 3x3 grid. They take turns putting their symbol (often
"X" and "O") in an empty space. The aim is to have three of your symbols in a row, either
horizontally, vertically, or diagonally, before your opponent. The first player to do this win. If
the grid is full and no one wins, the game ends in a draw.


Minimax Algorithm in Game Theory (Alpha-Beta Pruning):

Alpha-Beta pruning is not actually a new algorithm, but rather an optimization technique for
the minimax algorithm. It reduces the computation time by a huge factor. This allows us to
search much faster and even go into deeper levels in the game tree. It cuts off branches in the
game tree which need not be searched because there already exists a better move available. It
is called Alpha-Beta pruning because it passes 2 extra parameters in the minimax function,
namely alpha and beta.

Let’s define the parameters alpha and beta.
Alpha is the best value that the maximizer currently can guarantee at that level or above.
Beta is the best value that the minimizer currently can guarantee at that level or below.

Pseudocode:

function minimax (node, depth, isMaximizingPlayer, alpha, beta):

 if node is a leaf node:
 
 return value of the node

 if isMaximizingPlayer:
 
 bestVal = -INFINITY
 
 for each child node :
 
 value = minimax(node, depth+1, false, alpha, beta)
 
 bestVal = max( bestVal, value)
 
 alpha = max( alpha, bestVal)
 
 if beta <= alpha:
 
 break
 
 return bestVal
 
 else:
 
 bestVal = +INFINITY
 
 for each child node:
 
 value = minimax (node, depth+1, true, alpha, beta)
 
 bestVal = min (bestVal, value)
 
 beta = min( beta, bestVal)
 
 if beta <= alpha:
 
 break
 
 return bestVal
 
Sample Input/output:

![image](https://github.com/Plabon-Dutta/Tic_Tac_Toe_AI_Version/assets/79752960/3bc8dac9-0393-457f-b722-98058fd84207)

![image](https://github.com/Plabon-Dutta/Tic_Tac_Toe_AI_Version/assets/79752960/10981b3f-4cf6-44e5-a75b-154bf786410c)

Challenges:  
 
Building a Tic Tac Toe game with Minimax and Alpha-Beta Pruning can be tricky due to the complexity of these algorithms. Designing a user-friendly interface, optimizing the AI, and handling unexpected situations are also challenges. Balancing AI difficulty levels, maintaining clean code, and ensuring an enjoyable user experience are key. Thorough testing and potential integration into a larger project add to the complexity. 
 
Conclusion:  
 
Creating a Tic Tac Toe game using Minimax and Alpha-Beta Pruning techniques is a helpful exercise in AI and game development. It teaches us about adversarial search, decision-making, and optimization. Building a smart AI opponent demonstrates the power of these algorithms in strategic games. Alpha-Beta Pruning makes the AI efficient and competitive in a simple game like Tic Tac Toe. This project also helps improve problem-solving and programming skills, which are valuable for tackling more complex AI games and applications. Overall, it's a great way to learn about AI and gaming. 
