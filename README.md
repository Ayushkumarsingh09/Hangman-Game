# Hangman-Game
Implemented Hangman challenge using Trexquant API with accuracy >50%
Certainly! Here's a revised overview with some wording changes that could be suitable for a GitHub README or similar documentation:

# Trexquant Hangman Challenge

The provided Jupyter Notebook (`HangmanAPI.ipynb`) defines a Python class called `HangmanAPI`, designed as an interface for seamless interaction with a Hangman game API. This class encompasses various features to enhance gameplay strategy and communication with the API.

## 1. Initialization:
   - Upon instantiation, the class is configured with essential parameters like `access_token`, `session`, and `timeout`.
   - The `determine_hangman_url` method is employed to ascertain the appropriate Hangman game API URL.

## 2. Building Dictionaries:
   - A comprehensive dictionary of words is read from a file, and dynamic dictionaries based on word length are constructed using methods such as `build_dictionary` and `build_n_word_dictionary`.
   - The `full_dictionary_common_letter_sorted` attribute maintains a count of the most common letters found in the full dictionary.

## 3. Word and Letter Processing:
   - The class offers methods for tasks like counting vowels in a word (`vowel_count`) and processing words and letters to filter dictionaries (`func`, `func2`).

## 4. Game Logic:
   - The core of the Hangman game logic is encapsulated in the `guess` method. It intelligently makes guesses based on the ongoing game state and the available dictionaries.
   - The `start_game` method initiates a new Hangman game, makes educated guesses, and manages responses until the game concludes, either successfully or unsuccessfully.

## 5. API Communication:
   - To communicate with the Hangman API, the class employs a `request` method utilizing the `requests` library.
   - Robust error handling is implemented through a custom exception class called `HangmanAPIError`.

## 6. Exception Handling:
   - The `HangmanAPIError` class is specifically crafted to handle errors returned by the Hangman API effectively.

## 7. Other Methods:
   - The `my_status` method retrieves the current status of the Hangman game.

This class serves as a comprehensive toolkit for interacting with a Hangman game API, spanning from initialization to strategic guessing and response handling. The code is well-organized and includes comments for improved clarity. If you have specific inquiries or require additional explanations on particular sections, please feel free to inquire!
