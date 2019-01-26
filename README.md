# Pip_Puzzle
## THEME OF THE GAME ##

The main theme behind developing puzzle game using java is to provide a creative and competitive environment for the players who will use this system. 
The goal of this little game is to form a picture. 

## Framing of the Puzzle Game ##

1. Consider buttons with appropriate actions relevent to the game.
2. Buttons containing images are moved by clicking on them.
3. Only buttons adjacent to the selected start button can be moved.
4. We scale the image and cut it into 9 pieces. 
5. These pieces are used by JButton components.
6. You can download some reasonably large picture and use it in this game. 
7. We use a GridLayout to store our components.
8. The layout consists of 3rows and 3 columns.
9. All the components from the buttons list are placed on the panel. 
10. We create some gray border around the buttons and add a click action listener.
11. Buttons are stored in an array list. This list is then mapped to the grid of the panel. 
12. We get the indexes of the last button and the clicked button. They are swapped  if they are adjacent. 
13. Solution checking is done by comparing the list of points of the correctly ordered buttons with the current list containg the order of buttons from the window. 
14. A message dialog is shown in case the solution is reached.

## Methods Used in the Game ##
1. picpuzzle2():
	In this class every image is assigned to a variable. And the image which is used to swap in the whole game is assigned with a different variable.
	A constructor is called to set the buttons for every image and that are stored in another variable such that the action are performed by assigning the addActionListener(this). 
2. actionPerformed():
 	In this class the logic is implemented for the puzzle game like getSource() is to select the image to swap with the main image which is given permission to role around the given grid.
 	Then after swapping that image is called with getIcon() and this is the perfect picture to be assigned to that place then it is setted for setIcon().
3. main():
	The whole puzzle game starts here and pippuzzle2() is called here. 
