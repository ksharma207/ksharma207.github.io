# Random Guessing Game Flowchart

```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Get User Guess]
    C --> D{Is Guess Correct?}
    D -- No --> E[Show "Try Again"]
    D -- Yes --> F[Show "Correct"]
    E --> C
    F --> G[End]

Start: The game starts.
Generate Random Number: The computer generates a random number.
Get User Guess: The user enters their guess.
Check Guess:
If the guess is not correct, show "Try Again" and prompt for another guess.
If the guess is correct, show "Correct".
End: The game ends after the correct guess.

