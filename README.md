# Tombala Game
   A Tombala Game designed with Python and Qt Designer. In this project used Python's object oriented programming and Qt Designer's GUI features. 
 
 First of all, an interface with an .ui extension is designed for the game to be written with Qt Designer. The designed interface has a menu and a game screen. These two screens are on the same Main Window as the design and one is hidden while the other is visible.

The designed screen should be saved in a folder. Then the location where the interface designed from the command prompt should be opened. This is done with the following code.
For Windows:

```bash
C:\Users\Ceren> cd C:\Users\Ceren\path_where_the_file_is_located
```

Then, XML files obtained from Qt Designer with PyQt5 should be converted to Python code. We can do this using the code below.

```bash
C:\Users\Ceren> pyqt5 -x ui_file_name.ui -o python_file_name.py
```

The resulting Python code is only for the design of the .ui interface. Therefore, codes must be added for later features.

The codes given above are ready to use. Downloaded codes and images must reside in the same folder.

## Instructions
* Clone this repo.
* Run python tombala_driver.py.
* Play for play game.
* Exit to quit game.
* Enter {player1 name} {player2 name} to create a new room. Game will start after {countdown} seconds.
* Choose cards' colors
* Initialize numbers on cards
* Pick stamp
* Take stamp if there is a number on the card that matches the stamp

## Play Game

"Tombala" game was designed with Qt Designer and coded using Python programming language. When the game code is executed, we first encounter a menu shown in Figure-1, and there are two buttons: "Play" and "Exit". The "Exit" button causes the game to close, while the "Play" button directs it to the game. 


<p align="center">
  <br><br>
  <img src="https://user-images.githubusercontent.com/59059790/84407488-986f2b80-ac13-11ea-8566-4147b29fb44d.png">
</p>

Then we come across the main game interface shown in Game figure. In this interface, first of all, the names of the players should be written in the "Player 1" and "Player 2" text edits. Players should then choose the desired card color from the combo boxes provided and click on the "Initialize Numbers" button to be ready for the game. With the "Initialize Numbers" button, each row is sorted from small to large, 15 numbers are randomly selected in the 1-90 range. After the tombala cards are prepared, players should draw random numbers in the range of 1-90 using the "Pick Number" button and check whether this number is on their cards.

<p align="center">
  <br><br>
  <img src="https://user-images.githubusercontent.com/59059790/84412054-57791600-ac17-11ea-89d8-a84ae0560532.png">
  <br><br>
</p>

If the players find that the number drawn is on their cards, they must place the number drawn with the "Take Stamp" button, in the upper left corner of each card, in the correct place on their cards.

<p align="center">
  <br><br>
  <img src="https://user-images.githubusercontent.com/59059790/84426652-3ec72b00-ac2c-11ea-9d14-37e964b60162.png">
  <br><br>
</p>

Throughout the game, as the users place the numbers drawn in their correct positions, the lines on the cards will be completed. Each player gets 10 points for the first line he/she completed, 20 for the second line, and 40 for the third line, and the player who has reached 70 points in total has won the game. If players missed these stamps even though some of the numbers on their cards are equal to the number drawn, they cannot complete their cards and lose the game. If both players encounter this situation, the game ends with the end of 90 stamps to be drawn. 

<p align="center">
  <br><br>
  <img src="https://user-images.githubusercontent.com/59059790/84426301-a8930500-ac2b-11ea-9213-c5ce4b48acb2.png">
  <br><br>
</p>


When the game is over, players encounter a message box on the screen. This message box provides information about who won the game. There are two things that can be done when the game ends: The first is to quit the game, and the second is to return to the menu for the new game. To return to the menu, "Menu" should be selected from the "File" menu, shown in Figure-3, in the upper left corner of the game. Ctrl + X shortcut or "Exit" option under "File" menu can also be used to exit the game.

<p align="center">
  <br><br>
  <img src="https://user-images.githubusercontent.com/59059790/84426121-5eaa1f00-ac2b-11ea-8feb-bc9c59abe12b.png">
  <br><br>
</p>
