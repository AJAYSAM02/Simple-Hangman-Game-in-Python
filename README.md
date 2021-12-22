# Simple-Hangman-Game-in-Python
This is a very simple project made using Python.

## STEPS
### Importing the random and time modules
1. import random is used to randomly choose an item from a list [] or basically a sequence
2. import time is used to import the actual time from your pc to use in the program
3. time.sleep() is used to halt the execution of the program for a few seconds
### Defining functions with specific global arguments
1. we define the main function that initializes the arguments: global count, global display, global word, global already_guessed, global length and global play_game
2. words_to_guess contains all the Hangman words we want the user to guess in the game
3. word is used to randomly choose the word from words_to_guess in the game
4. len() helps us to get the length of the string
5. count is initialized to zero and would increment in the further code
6. display draws a line for us according to the length of the word to guess
7. already_guessed contains the string indices of the correctly guessed words
### Implementing loops to execute the program
1. play_loop() takes in the argument of play_game
2. play_game is used to either continue the game after it is played once or end it
3. while loop is used to execute the play_game argument
4. y-> game restarts n-> game ends
### Passing the function in the program to run
1. we call all the arguments again under the hangman() function
2. limit is the maximum guesses we provide to the user to guess a particular word
3. guess takes the input from the user for the guessed letter
4. guess.strip() removes the letter from the given word
5. If loop checks and tells the user about the invalid input and executes hangman again.
### Game
If the letter is correctly guessed, index searches for that letter in the word. Display adds that letter in the given space according to its index or where it belongs in the given word. If we have already guessed the correct letter before and we guess it again, It tells the user to try again and does not lessen any chances. If the user guessed the wrong letter, the hangman starts to appear which also tells us how many guesses are left. Count was initialized to zero and so with every wrong guess its value increases with one.
If the word is guessed correctly, matching the length of the display argument, the user has won the game. play_loop asks the user to play the game again or exit. main() and hangman() would start again if the play_loop executes to yes.
