# Random Guessing Game Flowchart

```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Get User Guess]
    C --> D{Is Guess Correct?}
    D -- No --> E[OOPS! Try Again]
    D -- Yes --> F[WOOHOOOO! You got it!]
    E --> C
    F --> G[End]
1. The game begins.
2. The program generates a random number.
3. The user enters their guess.
4. If the guess is not correct, show Try again and go back to Get User Guess.
If the guess is correct, show "Correct" and end the game.
5. The game ends.


