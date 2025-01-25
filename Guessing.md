# Random Guessing Game Flowchart

```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Get User Guess]
    C --> D{Is Guess Correct?}
    D -- No --> E[Try Again]
    D -- Yes --> F[Correct!]
    E --> C
    F --> G[End]



