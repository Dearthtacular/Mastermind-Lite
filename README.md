# Mastermind Lite

Thank you for selecting Mastermind Lite for all of your entertainment needs.  Mastermind Lite is playable in modern browsers and was created using JavaScript, HTML, and CSS.

For a history of the original Mastermind, please visit [wikipedia](https://en.wikipedia.org/wiki/Mastermind_(board_game)).

There are some distinct differences between the original Mastermind and Mastermind Lite:

Original Mastermind was created as a two player game.  Players score points only when they play the role of the code maker.  Since the role of code maker is filled by the computer in Mastermind Lite, another schema is necessary:

There are no points in Mastermind Lite.  Rather, the player _(the code breaker)_ has ten possible turns to guess the code generated by the computer _(the code maker)_.  If the code is guessed in ten turns or less, the player wins.  If the player does not guess the code in ten turns, the player loses.

Mastermind Lite does not keep track of rounds won, and there are no accumulated credits or totals from one playthrough to the next.  Mastermind Lite is designed to be a quick playing experience while providing an enjoyable challenge for the player.

## Concept:

At the launch of the game, the computer will automatically generate and hide a code of four colored squares for the player to guess.  The code can comprise any combination of the playable colors (multiple instances of the same color included).  The computer cannot have a blank or null as one of its color choices.

The goal of the game is for the player to guess the code generated by the computer by placing colored squares in the same vertical position as the computer's code.

## Instructions:

1. The player selects a color for each playable square by clicking repeatedly to toggle through all available color selections.  After selecting a color in each square, the player then clicks the __guess__ button to submit their guess for evaluation by the reporting function and advance to the next turn.  Note that the __guess__ button will not activate until the player selects a color for every playable square for the current turn.

    > The playable colors are:  firebrick, deepskyblue, olivedrab, gold, dimgrey, and lightpink.

2. Once the player clicks the "guess" button, the game will:
- Automatically display an empty row for the next turn
- Advance the row for the prior turn down the board
- Provide a report for the accuracy of the guesses in the prior turn.  The report will appear to the left of the prior turn's row in a matrix of four possible report dots

The report dots have the following meanings:

>![green dot](images/greendot.png)
Green: The player selected a color that appears in the correct vertical position relative to the code makers' code.

>![orange dot](images/orangedot.png)
Orange: The player selected a color that appears somewhere in the code makers' code, but it is located in an incorrect vertical position.

>No dot / dot absent:  The player selected a color that is not present in the code maker's code.

<br>

__Note__: The report dot locations are not fixed relative to the vertical locations guessed by the player.  In other words, if a guess yields a green dot in the __upper left__ quadrant of the reporting field, an _identical_ guess may yield a green dot in the __lower right__ quadrant of the reporting field.  All dot locations are randomized each turn, but the same information is conveyed.

## Examples

### Turn one

![turn 1](images/turn1.png)

The player selected four random colors.  The report states that two colors present in the player guess are in the code makers code, with one in the correct location (green dot) and one in an incorrect location (orange dot).

### Turn two

![turn 2](images/turn2.png)

The player selected three of the four colors chosen in turn one and added one more to the row.  The color that resulted in a green dot in turn one has either moved or been removed.

### Turn three

![turn 3](images/turn3.png)

and so on...

Upon completing the game (win or lose), the code created by the computer is revealed.

![win screen](images/win.png)

## Icebox Items

There are future options that are designed to adjust the level of difficulty for the player:

1. The ability to select no color (blank) as a guess option
2. Similar to the ability to select no color, the ability to add colors to the palette of possible guess options
3. The ability to increase or decrease the number of guess rows (turns) per game

## Credits

Background image by <a href="https://www.freepik.com/free-vector/gradient-futuristic-background-with-connection-concept_18777126.htm#query=electronic%20background&position=2&from_view=keyword&track=ais&uuid=2c59befd-5342-4f3b-94f5-05b6ccb80e80">Freepik</a>