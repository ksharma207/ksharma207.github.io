# Random Guessing Game Flowchart

```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Get User Guess]
    C --> D{Is Guess Correct?}
    D -- No --> E[OOPS! Try Again]
    D -- Yes --> F[WOOHOOOO! You got it!]
    E --> C
    F --> G[End]```

