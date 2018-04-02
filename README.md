# windmill-tilting
don quixote gets around a chessboard and touches all the things.

#---------------------------------------------------------------#
|              A Knight's Tour via Stacks & Queues              |
#---------------------------------------------------------------#

A Knight's Tour is a sequence of moves of a knight on a chessboard such that the knight visits every square once and  only once. If the knight ends on a square that is one knight's move from the beginning square (so that it could tour the board again immediately, following the same path), the tour is closed, otherwise it is open.

The Knight's Tour Problem is the mathematical problem (http://math.oregonstate.edu/~math_reu/proceedings/REU_Proceedings/Proceedings2002/2002AL_McGown.pdf) of finding a knight's tour. Creating a program to find a Knight's Tour is a common problem given to computer science students at every major university. Normally, it is given in an introductory course in order to teach recursion. When using recursion, "backtracking" is accomplished via the run-time stack. An article on backtracking can be found here:  https://en.wikipedia.org/wiki/Backtracking.

Warnsdorff's rule:
Each square contains an integer giving the number of moves that the knight could make from that square. In this case, the rule tells us to move to the square with the smallest integer in it, namely 2. Warnsdorff's rule is a heuristic for finding a knight's tour. We move the knight so that we always proceed to the square from which the knight will have the fewest onward moves. When calculating the number of onward moves for each candidate square, we do not count moves that revisit any square already visited. It is, of course, possible to have two or more choices for which the number of onward moves is equal; there are various methods for breaking such ties, including one devised by Pohl and another by Squirrel and Cull.
 
The heuristic was first described in "Des Rösselsprungs einfachste und allgemeinste Lösung" by H. C. von Warnsdorff in 1823. Even to this day,Computer Scientists are expanding upon this rule.

See: http://mathworld.wolfram.com/KnightsTour.html or 

The Task:

In teams of two, develop a program that will solve the Knight's Tour for any starting position given by the end-user on a standard chessboard, in standard chess notation. Your program with then print, in standard chessboard nomenclature, the moves that the knight must take to touch each square once and only once. After displaying the moves, your program should state whether the solution it provided is either open or closed. Additionally, since you have already done recursive programs in the pre-requisite courses, you must implement backtracking in two different methods. First, by using a stack (implemented as a linked list) that you've developed, and then secondly, with a queue (priority queue implemented as an array) that you've developed. Run times for each of these methods must be calculated and displayed. Your program must also offer the end-user the ability to print the tour as well as re-run the tour with a different starting point.

Standard chess nomenclature can be found at (https://en.wikipedia.org/wiki/Chess_notation).

On the due date, you and your partner must demonstrate your program during lab. Printouts of your code must be submitted at the time of demonstration. As in the printer in R211 is not functioning, you must bring printouts prior to class!


Extra Credit:

- Graphically show the movements of the knight on the chessboard after the tour has been calculated. This must be done on an 8 x 8 chessboard. (50 points)
- Calculate all possible closed Kinight's Tours (50 points)
- Have the end-user enter a starting point and an ending point on the chessboard and have the program calculate a Knight's Tour between the two points (50 points)
