# UMBC Wordle Project
First project written in the Computer Science I course (CMSC202) at the University of Maryland, Baltimore County (UMBC). 
This project was written using C++ by Andrew Chen and was submitted on March 1st.

# What is Wordle?
The Wordle Project is based on the well-known word guessing game, Wordle. The original game
was created by a Welsh software engineer, Josh Wardle. The game works by allowing players
a limited amount of guesses, usually six guesses. Players win the game by guessing the word
correctly before they run out of guesses. They lose when they don't guess the word within the
number of guesses they are given. The game also provides hints that help players towards
guessing the correct word.

# How to run
Running the game is simple, just double click 'wordle.exe' to start playing.

NOTE: 'wordle.exe' and 'proj1_data.txt' MUST be in the same folder or the game
will not run without the text file.

# How to Play
## Here are some rules:
- You have 6 attempts at guessing the word correctly
- You win by guessing the word correctly before the sixth guess
- You lose by not guessing correctly by the last guess
- The word you guess MUST be 5 letters long
- Try not to cheat by looking inside the word list .txt file

## Mechanics:
When you start, this will be your start screen:

``` 
Welcome to UMBC Wordle!
Your file was imported!
12971 words imported.
Ok. I am thinking of a word with five letters
GUESS #1
What word would you like to guess?
_
```
If you enter a word that isn't five letters long, the game will prompt you to
try again:

```
What word would you like to guess?
use
That word is not in the word list
What word would you like to guess?
_
```
However, if you enter a valid word, the game will show you the results of your guess:
```
What word would you like to guess?
raise
You guessed: raise
&_!&_
-----
-----
-----
-----
-----
```
In Wordle, there are hints that tell the player whether they are on the right track or not. In the original game, a letter highlighted as GREEN means that the letter is part of the word and is in the correct spot. A letter highlighted as YELLOW means that the letter exists within the word, but the letter is not in the right spot. Finally, a letter highlighted as GRAY means that it isn't part of the word at all.

Now, in this version of Wordle, there is no color coding. Instead we have the symbols of '&' , '!' , and '_'. This is what each symbol represents:
- ! : The letter exists in the word and is in the right spot
- & : The letter exists in the word but is not in the right spot
- _ : The letter doesn't exist within the word at all

Looking back at the example:
```
What word would you like to guess?
raise
You guessed: raise
raise
&_!&_
-----
-----
-----
-----
-----
```
We can see that 'r' and 's' is in the word but not in the correct spot depicted by the '&'. The letter 'i' is in the word and is in the right place shown by the '!'. Finally the letters 'a' and 'e' do not exist in the word at all. Using these hints, the player will be able to (hopefully) guess the correct word.

The game will continue working in this manner and the player's screen will eventually look like this:
```
GUESS #1
What word would you like to guess?
raise
You guessed: raise
raise
&_!&_
-----
-----
-----
-----
-----
GUESS #2
What word would you like to guess?
obese
You guessed: obese
raise
&_!&_
obese
___&_
-----
-----
-----
-----
GUESS #3
What word would you like to guess?
bloat
You guessed: bloat
raise
&_!&_
obese
___&_
bloat
_____
-----
-----
GUESS #4
What word would you like to guess?
_
```
## Winning Screen
This message should appear when you win:
```
Congrats you won!
The correct word was: shule
Please wait 24 hou- Jk.
Another game? y/n
```

## Losing Screen
If you lose, this message should appear:
```
The correct word was: speil
Please wait 24 hou- Jk.
Another game? y/n
```

## Play again
After the round ends, the game will ask if you would like to play another round. Entering 
'y' will start a new round, while entering 'n' will close the game.

## Customization
The default word list text file (named proj1_data.txt) contains 12971 words that
the game will choose from. The player may edit the word list file to add/ remove
words from the text file. 

IMPORTANT: Underneath the last word in text file, make 
sure to leave an empty line. So for example:
```
.....   .....
12970   zymes
12971   zymic
12972   (Nothing should be printed on this line)
```
# Flowchart
In progress
# UML Chart
In progress
# Notes
If you want a more thorough demonstration of this game, please view [proj1_sample.txt](https://github.com/AChen342/UMBC-Wordle-Project/blob/master/proj1_sample.txt)