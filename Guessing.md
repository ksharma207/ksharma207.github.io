# Random Guessing Game Flowchart

```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Get User Guess]
    C --> D{Is Guess Correct?}
    D -- No --> E[Try Again]
    D -- Yes --> F[Correct]
    E --> C
    F --> G[End]

Start: The game begins.
Generate Random Number: The program generates a random number.
Get User Guess: The user enters their guess.
Check Guess:
If the guess is not correct, show "Try Again" and go back to Get User Guess.
If the guess is correct, show "Correct" and end the game.
End: The game ends.

