# snakeGame

Description:
The program is based on the basic concepts of Snake Game and is written in C++
*It is fully functional on DevC++ ide.

Working And Basic Idea:

Here the approach is not to map or plot the snake and it's body,
*The whole canvas or Game Area is a 2D array of Character type
*The snake body is actually a list [Data Structures(Basic concept of lists)]
   *the individual node of the list comprises of CharacterSymbol(0-head ,o-body) , RowIndex , ColumnIndex ,Address Of Next Node 
 
 *When Game starts:
    -The 2D array is initialized with it's border rows with | and - to create border and the rest array is filled with ' ' (whitespaces)
    -The root node of the list is created and has the default address for the snake's head
    -The root node is displayed on the 2D array by the RowIndex and ColumnIndex stored in it, initialized to the 2D[RownIndex][ColumnIndex]
    -The fruit is assigned randomly to the 2D array
    -***When the head meets the fruit new node is appended to the list, now as soon as the snake head moves the currently 
        stored RowIndex and ColumnIndex are transferred to the following node in the list until the end[NULL] is reached 
        and the last index positions are equalised to ' ' [BlankSpace], while the new head index is stored in the root node,
        thus moving the snake
    
Key Notes:
This approach to the SnakeGame is the publisher's original idea and thus may not be the best or most efficient way to implement the game, contribute to it on your own interests.
Contributors are always welcome to raise queries over the code in case of any confusions.
