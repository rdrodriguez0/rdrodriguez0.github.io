``` mermaid
  flowchart TB
    A[Start] e1@--> B[Generate Random Number 1- 100]
    e1@{ animate: true, animation: slow }
    B --> C[Prompt User for a Guess]
    C --> D{Is Input a Number?}
    D -- No --> E[Show: ERROR!] --> C
    D -- Yes --> F{Determines if it's a number and if it's the correct number or not}
    F -- Yes --> G[Show Message: CORRECT!Winner Winner!]
    F -- No --> J[Hint: Too High / Too Low]
    G --> H[Ask to Play Again?]
    H -- Yes --> B
    H -- No --> K[End Game]
    J --> C
```


## Number Guessing Game Flowchart

The chart above shows the flow of the Number Guessing Game. Below is a legend and details on what occurs.

#### **Legend**

* A: Start
* B: Generate Random Number 1-100
* C: Prompt User for a Guess
* D: Is Input a Number
* E: Show Error: Invalid Input
* F: Is Guess Correct
* G: Show Message: Correct Guess!
* H: Ask to Play Again?
* I: Hint: Too High / Too Low
* J: Show Message: GAME OVER!
* K: End Game

#### **Details of Flowchart**

1. Once the game starts with "**A**" and go to "**B**".
2. Next, "**B**" will generate a number from 1-100 and go to "**C**".
3. On "**C**", it will have the user make a guess at a number and go to "**D**". 
4. "**D**" will then determine if the output is a number or not.
5. If the user's guess is not a number, it will go to "**E**", which will then begin from "**C**" again.
6. If the user's guess is a number, it will go to "**F**".
7. From "**F**", it will determine if the user's number guess was correct or not.
8. If yes, then it would go to "**G**" and display an _**CORRECT! Winner Winner!**_.
9. If not, it will give the user a *HINT* whether the number is *too high* or *too low* and go back to "**C**"
10. This will continue to occur until the user guesses the correct number, then go to "**H**"
11. "**H**" will then *ask to PLAY AGAIN?*
12. If yes, it will start all over and go to "**B**"
13. If no, it will go to "**J**" and display the message of *GAME OVER!* and go to "**K**" which will end the game.





