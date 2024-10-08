<div align="center">
<pre>
  _        ___   ___   ___   _     ____       __    _ 
 \ \    / / / \ | |_) | | \ | |   | |_       / /\  | |
  \_\/\/  \_\_/ |_| \ |_|_/ |_|__ |_|__     /_/--\ |_|
 -------------------------------------------------------
Intelligent Word Guessing in C
</pre>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

</div>

Welcome to Wordle AI! This C program presents a unique twist on the popular word-guessing game, Wordle! In this program, the tables turn as you, the user, become the mastermind behind the secret word while the computer takes on the challenge of guessing your chosen word. The program's goal is to guess the secret word through intelligent guesswork and intricate scoring mechanisms.

## How it Works

1. **Word Selection**: The program can accept either a user-inputted secret word or randomly choose one from a provided word list.
2. **Scoring Mechanism**: The AI utilizes a scoring mechanism to refine its guesses and improve accuracy by comparing word similarity and positions.
   - Exact Letter Matches: Correct letters in the correct position are colored green and displayed in uppercase. For each correct letter in the correct position, the score for related words is increased.
   - Partial Letter Matches: Letters in the secret word but not in the correct position are colored yellow and displayed in uppercase. Partial matches help narrow down possibilities but aren't in the correct positions, influencing the AI to reconsider letter placements.
   - No Letter Matches: Letters in the guessed word that do not match any letter in the target word are displayed lowercase and receive a negative score.
3. **Iteration & Refinement**: The AI continuously refines its guesses based on the accumulated scores, discarding less likely words and favoring those with higher scores.

## Example Execution
![7802F974-8895-4EBE-ABC7-2D5C223DE4A6](https://github.com/user-attachments/assets/7eca74fa-87c1-46ee-b77b-3f573acf8598)
![A8280844-7563-4288-8B88-F381C012FD45](https://github.com/user-attachments/assets/fc56b19e-8c31-4754-a6bf-5cccd2c202b3)


## Files Included

- `main.c`: The main C file containing the Wordle AI logic.
- `wordsLarge.txt`: File containing a substantial 5-letter word list used for guessing.
- `wordsTiny.txt` (commented out): Smaller 5-letter word list used for debugging purposes.

## Running the Program
When you execute the program, follow these steps to interact with the game:

1. Compile the Program:
- Compile the program using a C compiler (e.g., GCC).
- For example: gcc main.c -o wordle_ai

2. Run the Program:
- Execute the compiled program.
- For example: ./wordle_ai

3. Follow Game Instructions:
- Provide a secret word or select 'r' for a random word to be given to the computer.
- Observe the AI's guessing process and scoring until the secret word is found.
- The program runs the guessing process three times, using the previous secret word as a starting guess word with each iteration.


