```mermaid
flowchart TD
    A[Start Game] --> B[Generate Random Number]
    B --> C[Prompt Player: Guess a Number]
    C --> D{Is Guess Correct?}
    D -- Yes --> E[Display: "You Win!"]
    D -- No --> F{Is Guess Higher or Lower?}
    F -- Higher --> G[Display: "Too High! Try Again."]
    F -- Lower --> H[Display: "Too Low! Try Again."]
    G --> C
    H --> C
    E --> I[End Game]
    ```