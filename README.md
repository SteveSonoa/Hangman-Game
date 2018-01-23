# An Introduction to Super Mario Hangman!
This represents the first interactive project I’ve ever created in JavaScript. It was an exercise in array manipulation, so the selected words were stored in a large array. In addition, I used dynamic arrays to hold the individual letters of the completed word, the player’s status showing how many letters have been correctly guessed, and another array of previously guessed letters.

For input validation, only letters are accepted; upper case and lower case are seen as the same. Typing a letter that has already been guessed won’t count against you.

When the project was completed, I was challenged to include sound effects. The results were so much fun, I decided to add sound effects to the next several projects in abundance!

### How does it work?
The words are selected from a master array; each word is split into its individual letters, then another array is created to be the same length, but only including underscores. This is the game state array.

There is a main listener event that waits for keystrokes. It checks to see if they keystroke is a letter, then it goes through the arrays to first see if the typed letter has already been guessed; if it hasn't, it will go through the solved array to see if there's a matching letter. If it finds a match, it will splice the game state array by removing the underscore at the appropriate index and replace it with the correct letter.

When there are no more underscores, the player wins! If the player runs out of guesses, the game is over in a loss. Wins and losses are stored locally.

### Who will use this?
Nintendo fans have all enjoyed playing the game. Without a keyboard, the game cannot be played on mobile devices; this app is limited to computers only.

### What is the goal?
The goal was to use event listeners and validate user input in real time. I took the extra challenge of adding sound effects to various game aspects, which had fantastic results.

# Deployment
The code can be used in most web servers; there is no required node or database requirement.

# Screenshot
![Screenshot](http://www.fullstacksteve.com/wp-content/uploads/2015/06/hero-mariohangman.png)

# Credits
Steve Marshall, Sole Developer
* [Steve's Online Portfolio](http://fullstacksteve.com/)
* [Steve's LinkedIn Profile](https://www.linkedin.com/in/sonoa/)