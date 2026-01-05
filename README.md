# Learning to Play Tic-Tac-Toe 🎮

<table align="center">
  <tr>
    <td width="50%" align="center">
      <img 
        src="https://github.com/user-attachments/assets/355071bc-2857-4b0a-8c87-e9be53de94a0"
        width="100%"
        style="max-height:420px; object-fit:contain;"
      >
    </td>
    <td width="50%" align="center">
      <img 
        src="https://github.com/user-attachments/assets/aa3ff9d5-3cb3-412e-a859-4558f0ecd106"
        width="100%"
        style="max-height:420px; object-fit:contain;"
      >
    </td>
  </tr>
</table>




This project shows how a computer program can learn to play Tic-Tac-Toe *from experience*, rather than by following hard-coded rules. Starting with no strategy at all, the agent plays thousands of games, learns from wins and losses, and gradually improves its decision-making over time.


---

## What’s the idea?

Imagine learning Tic-Tac-Toe by:
- trying random moves,
- remembering which choices led to wins,
- avoiding moves that caused losses.

That’s exactly what this program does.

The agent keeps track of past game situations, favors moves that worked well before, and slowly builds a better strategy as it plays more games. Over time, you can actually *see* it getting better.

---

## How the learning works 

- The agent plays games of Tic-Tac-Toe against an opponent.
- After each game, it gets feedback:
  - **Win** → reward good moves  
  - **Draw** → small reward  
  - **Loss** → discourage bad moves
- Moves that lead to good outcomes become more likely in the future.
- Moves that lead to bad outcomes become less likely.

This simple feedback loop is repeated thousands of times, which allows learning to emerge naturally.

---

## What’s included in this project

- A full Tic-Tac-Toe game engine (board, rules, win conditions)
- A self-learning agent that improves through experience
- Large-scale simulations (tens of thousands of games)
- Learning curves that show performance improving over time
- A baseline comparison against a non-learning (random) player

---


## Tools used

- Python  
- NumPy  
- Matplotlib  

(No machine learning libraries were used—the learning logic was implemented from scratch.)

---

## Notes & limitations

- The agent does not account for board symmetries, meaning it has to learn similar situations multiple times.
- Because of this, learning is slower than it could be—but the behavior is easier to observe and understand.

---

## Want to explore more?

Some fun extensions you could try:
- Teaching the agent to recognize symmetric board positions
- Playing it against a smarter opponent
- Visualizing move probabilities over time

---

Thanks for checking out the project! 🙂
