# Hangman Game 🎮

A classic Hangman word-guessing game implemented in Python. Try to guess the hidden word before you run out of lives!

## Project Overview

This is a terminal-based implementation of the traditional Hangman game where:
- A random word is selected from a word list
- The player has 6 lives to guess the word correctly
- Each incorrect letter costs one life
- The player wins by revealing all letters before losing all lives
- ASCII art shows the hangman's progression with each wrong guess

## Files

- **`main.py`** - Main game logic and gameplay loop
- **`hangman_words.py`** - Contains the word list used for random word selection
- **`hangman_art.py`** - ASCII art for the hangman stages and game logo

## How to Play

1. Run the game:
   ```bash
   python main.py
   ```

2. You'll see the hangman logo and a placeholder with underscores for each letter

3. Guess one letter at a time when prompted

4. For each correct guess, the letter will be revealed in the word

5. For each incorrect guess:
   - You lose one life
   - The hangman drawing progresses
   - You have 6 lives total

6. **Win condition**: Reveal all letters in the word before losing all lives

7. **Lose condition**: Run out of lives before guessing all letters

## Game Features

- **Random word selection** from a comprehensive word list
- **Visual feedback** through ASCII hangman art
- **Life counter** showing remaining attempts
- **Duplicate guess detection** - prevents re-guessing the same letter
- **Case-insensitive** - works with uppercase and lowercase letters
- **Win/Loss announcements** - clear game ending messages

## Requirements

- Python 3.x

## Installation

1. Clone or download the project
2. Navigate to the project directory:
   ```bash
   cd hangman_game
   ```
3. Run the game:
   ```bash
   python main.py
   ```

## Example Gameplay

```
 _
| |
| |__   __ _ _ __   __ _ _ __ ___   __ _  _ __
| '_ \ / _` | '_ \ / _` | '_ ` _ \ / _` || '_ \
| | | | (_| | | | | (_| | | | | | | (_| || | | |
|_| |_|\__,_|_| |_|\__,_|_| |_| |_|\__,_||_| |_|

Word to guess: _ _ _ _ _ _
****************************6/6 LIVES LEFT****************************
Guess a letter: e
```

## Game Logic Flow

1. Initialize game state with a random word
2. Display the game logo and empty word placeholder
3. Loop until game is over:
   - Display current lives and hangman stage
   - Prompt player for letter guess
   - Check if letter is in the word
   - Update display with correct guesses
   - Deduct lives for incorrect guesses
   - Check for win (all letters revealed) or lose (0 lives remaining)
4. Display final result

## Future Enhancements

- Difficulty levels with different word categories
- Score tracking across multiple games
- Custom word list input
- Multiplayer mode
- GUI implementation
- Hints system

## License

Free to use and modify.

---

Enjoy the game! 🎯
