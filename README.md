# 🎲  Dice Game

dice game built with **HTML, CSS, and JavaScript**. Two players take turns rolling a die, racking up points — but roll a 1, and you lose everything you earned that turn!

## 📜 Game Rules

- Two players take turns rolling a single die.
- On each turn, a player repeatedly rolls the die:
  - If the roll is **2–6**, it's added to the player's **current score** for that turn.
  - If the roll is **1**, the player loses all points accumulated in that turn, and play passes to the other player.
- At any point, a player can choose to **Hold**:
  - Their current turn score is added to their **total score**.
  - Play then passes to the other player.
- The game continues until a player reaches the winning score (intended to be a target like 100 — see [Roadmap](#-roadmap)).

## ✨ Features

- Turn-based two-player gameplay
- Dice roll with matching dice face image
- Running "current score" tracker per turn
- Visual highlight for the active player
- New Game / reset functionality

## 🛠️ Built With

- **HTML** – structure
- **CSS** – styling and active-player highlighting
- **JavaScript** – game logic and DOM manipulation

## 📂 Project Structure

```
pig-game/
├── index.html      # Main HTML page
├── style.css        # Styling
├── script.js         # Game logic
├── imgs
└── README.md         # Project documentation
```


## 🧩 How to Play

1. Player 1 starts. Click **Roll Dice** to roll.
2. Keep rolling to add to your current turn score.
3. If you roll a **1**, you lose your current turn score and it becomes the other player's turn.
4. Click **Hold** to bank your current turn score into your total score and pass the turn.
5. Click **New Game** at any time to reset scores and start over.

## 🔧 Key Elements (`script.js`)

| Function / Variable | Purpose |
|---|---|
| `random_Number()` | Generates a random roll between 1 and 6 |
| `.btn--roll` handler | Rolls the die, updates the dice image, adds to current score or resets on a 1 |
| `.btn--hold` handler | Banks current score into total score, switches active player |
| `.btn--new` handler | Resets scores and starts a fresh game |
| `active()` | Toggles the `.player--active` class to highlight whose turn it is |

