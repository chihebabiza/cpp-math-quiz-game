# Math Quiz Game

This is a simple math quiz game implemented in C++. The game allows users to answer randomly generated math questions based on selected difficulty levels and operations.

## Features
- Choose from different difficulty levels: Easy, Medium, Hard, or Mixed.
- Select the type of operation: Addition, Subtraction, Multiplication, Division, or Mixed.
- Randomly generated numbers for questions based on difficulty level.
- Tracks the number of right and wrong answers.
- Displays final results (Pass/Fail) based on performance.
- Option to replay the game.

## Requirements
- C++ compiler (GCC, Clang, MSVC, etc.)
- Standard C++ library

## How to Play
1. The game will prompt you to enter the operation type:
   - 1: Addition
   - 2: Subtraction
   - 3: Multiplication
   - 4: Division
   - 5: Mixed operations
2. Select the question difficulty level:
   - 1: Easy
   - 2: Medium
   - 3: Hard
   - 4: Mixed
3. Enter the number of questions (between 1 and 10).
4. Answer each question displayed on the screen.
5. At the end of the game, the final results will be displayed.
6. Choose whether to play again or exit the game.

## Code Structure
- `RandomNumber(int from, int to)`: Generates a random number within a given range.
- `ReadNumberInRange(string message, int from, int to)`: Reads an integer input within a specific range.
- `enOperation`: Enum for operation types (Addition, Subtraction, Multiplication, Division, Mixed).
- `enLevel`: Enum for difficulty levels (Easy, Medium, Hard, Mixed).
- `stGameInfo`: Structure to store game details (Right/Wrong answers, Operation, Level, etc.).
- `stRoundInfo`: Structure to store round details (whether the answer is right or wrong).
- `PlayGame()`: Main function to run the game logic.
- `RunGame()`: Starts the game loop with replay functionality.
- `ClearScreen()`: Clears the terminal screen.

## Example Gameplay
```
Enter operation type (1:sum, 2:sub, 3:mul, 4:div, 5:mix): 1
Enter question level (1:easy, 2:mid, 3:hard, 4:mix): 2
Enter number of questions (1/10): 3

Question[1/3]
12 + 8 = 20
Right Answer

Question[2/3]
15 + 5 = 19
Wrong Answer

Question[3/3]
10 + 6 = 16
Right Answer

Final Result is PASS
Number of questions: 3
Question Level: Mid
Operation Type: Sum
Number of Right Answers: 2
Number of Wrong Answers: 1

Do you want to play again? (y/n): n
```

## License
This project is open-source and can be modified or distributed freely.

