
# 📘 Assignment: Hangman Game

## 🎯 Objective

Build a classic Hangman game in Python using strings, loops, and conditionals while creating an interactive guessing experience for the player.

## 📝 Tasks

### 🛠️ Word Selection and Game State

#### Description
Create the game setup so a random word is chosen and the player can see their progress as they guess letters.

#### Requirements
Completed program should:

- Store a list of words for the game to choose from.
- Randomly select one word at the start of each round.
- Display the hidden word using blanks such as `_ _ _ _ _` for unguessed letters.
- Track the letters that have already been guessed.
- Keep count of the remaining incorrect guesses.

### 🛠️ Guessing and End Conditions

#### Description
Implement the main game loop so the player can submit guesses until the word is solved or the game ends.

#### Requirements
Completed program should:

- Ask the player to enter a letter guess.
- Reveal matching letters in the hidden word when the guess is correct.
- Decrease the remaining attempts when the guess is incorrect.
- Prevent repeated guesses from counting twice.
- End the game when the player guesses the full word or runs out of attempts.
- Display a clear win or lose message at the end.
- Example gameplay:
  ```python
  _ _ _ _ _
  Enter a letter: a
  a _ _ _ _
  Enter a letter: e
  a _ _ _ e
  ```
