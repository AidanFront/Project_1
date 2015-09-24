#MEMORY CARD GAME

This is the classic memory game with a New Zealand theme.
The game may be played solo or with 2 players.

##Website

[aidanpartington.github.io/Project_1](http://aidanpartington.github.io/Project_1/)


##The rules

* Player may only turn 2 cards at once.
* If the two cards are not identical they will turn back over after 3 seconds.
* If the 2 cards match they will be paired and will not turn back over.
* Once all cards have been successfully paired the game will end and the score will be recorded.
* Each time 2 cards are turned over 1 turn is recorded.
* Changing player number or clicking 'RESET' at anytime will end and reset the game.
* If played 2, 'Player 1' will play first and score will be recorded. 'Player 2' will play second and scores will be compared to determine the winner.

##Aim of the game

The aim of the game is to test the user's memory. During the 3 seconds in which the card is revealed the user has time to commit images and location to memory. The goal is to pair all cards in the minimum amount of turns.

### Experience, Tech, bumps in the road

__Styling__ <br>
Playing with the transform function on different axises was very useful to create the desired flip animation.  <br>
It was interesting styling different sized images as backgrounds to standard square boxes. It needed to be done in such a way that every picture regardless of dimension would fit and render nicely within each card/box.


__Javascript__<br>
I was pleasantly surprised to find I really loved coding in Javascript. The games logic could be coded in a huge variety of ways. 

The logic I used was the following;<br>
I created a JS object that mirrored the markup div's. When a card was turned for the first time, it would be assigned a random class (which assigned an image), JS would then assign a corresponding string to the mirror. The mirror JS object is used as a record to make sure when a card is subsequently turned, cards kept the same image, and that only 2 of that particular image is assigned.  

The setTimeout function was used to make the image change exactly  at the halfway point during the transform animation. This gave the illusion that the card was turning over.

__Markup__<br>
The HTML markup was fairly straight forward with most of the effort put into setting up the grid.