```mermaid
flowchart TD
 A[Start Game] --> B[Generate Random Number]
    B --> C[Set Guess Count to 0]
    C --> D[Prompt Player: Guess a Number]
    D --> E[Increase Guess Count by 1]
    E --> F{Is Guess Correct?}
    F -- Yes --> G[Display: "You Win!"]
    F -- No --> H{Guess Count < 5?}
    H -- Yes --> I{Is Guess Higher or Lower?}
    I -- Higher --> J[Display: "Too High! Try Again."]
    I -- Lower --> K[Display: "Too Low! Try Again."]
    J --> D
    K --> D
    H -- No --> L[Display: "Game Over! You've used all your guesses."]
    G --> M[End Game]
    L --> M
    ```