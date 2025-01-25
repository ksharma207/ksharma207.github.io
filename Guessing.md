# Random Guessing Game Flowchart

```mermaid
flowchart TD
    Start([Start]) --> GenerateRandomNumber[Generate Random Number in Range]
    GenerateRandomNumber --> GetUserGuess[Get User Guess]
    GetUserGuess --> ValidateInput{Is Input Valid?}
    ValidateInput -- No --> ShowError[Show Error: Invalid Input] --> GetUserGuess
    ValidateInput -- Yes --> CompareGuess{Is Guess Correct?}
    CompareGuess -- Too Low --> ShowLow[Show 'Too Low'] --> GetUserGuess
    CompareGuess -- Too High --> ShowHigh[Show 'Too High'] --> GetUserGuess
    CompareGuess -- Correct --> ShowCorrect[Show 'Correct Guess!'] --> End([End])

Start: The program begins.
Generate Random Number: The computer generates a random number within a specified range.
Get User Guess: The user inputs their guess.
Validate Input: The program checks if the input is valid (e.g., numeric and within the specified range).
If invalid, it displays an error message and prompts the user to guess again.
Compare Guess: The program compares the user’s guess to the random number.
If the guess is too low, the program displays "Too Low" and asks for another guess.
If the guess is too high, the program displays "Too High" and asks for another guess.
If the guess is correct, the program displays "Correct Guess!" and ends.
End: The program terminates.
