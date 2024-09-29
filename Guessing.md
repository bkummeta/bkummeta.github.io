flowchart TD
    Start([Start]) --> A[Generate a Random Number within the range]
    A --> B[Prompt User to Guess a number]
    B --> C{Is Input Valid?}
    C -- No --> D[Display Please enter a valid number]
    D --> B
    C -- Yes --> E{Is Guess Correct?}
    E -- Yes --> F[Display Congratulations! You guessed it right!]
    F --> G[End Game]
    E -- No --> H{Is Guess Too High?}
    H -- Yes --> I[Display Your guess is too high! Try again]
    I --> B
    H -- No --> J[Display Your guess is too low! Try again]
    J --> B
    G --> End([End])
