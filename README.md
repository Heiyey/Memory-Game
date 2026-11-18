# 🎮 Memory Card Game

A card-matching memory game built with React and Vite. Flip two cards at a time to find all 8 fruit pairs, in as few moves as possible.

**🔗 Live demo:** [memory-game-sand-omega.vercel.app](https://memory-game-sand-omega.vercel.app/)

## Features

- 16-card board (8 emoji pairs) shuffled with the **Fisher–Yates algorithm** on every new game
- **Score** (pairs found) and **move** counters
- Board locks while two cards are face up, so you can't click a third card mid-turn
- Matching pairs stay revealed; non-matching cards flip back after a short delay
- Win message showing your total moves
- **New Game** button to reshuffle and reset

## How to Play

1. Click a card to reveal it.
2. Click a second card to try to match it.
3. If they match, they stay face up. If not, both flip back.
4. Match all 8 pairs to win. Try to beat your move count!

## Tech Stack

| Area | Tools |
|---|---|
| UI | React 19, CSS |
| State & logic | React hooks (`useState`, `useEffect`) in a custom hook |
| Tooling | Vite, ESLint |
| Deployment | Vercel |

## Getting Started

**Prerequisites:** Node.js 18+ and npm.

```bash
# Clone the repo
git clone https://github.com/Heiyey/Memory-Game.git
cd Memory-Game

# Install dependencies
npm install

# Start the dev server
npm run dev
```

Then open the URL Vite prints (usually `http://localhost:5173`).

Other scripts:

```bash
npm run build     # production build
npm run preview   # preview the production build locally
npm run lint      # run ESLint
```

## Project Structure

```
src/
├── components/
│   ├── Card.jsx          # A single flippable card
│   ├── GameHeader.jsx    # Title, score, moves and New Game button
│   └── WinMessage.jsx    # Shown when all pairs are matched
├── hooks/
│   └── useGameLogic.js   # Shuffling, flip/match rules, score, moves, board lock
├── App.jsx               # Wires the hook to the components
└── main.jsx              # Entry point
```

## What I Practiced

- Pulling game logic out of the UI into a **custom React hook** (`useGameLogic`)
- Managing related state (cards, flipped, matched, score, moves, lock) without race conditions
- Using timeouts for flip-back and match animations
- Breaking the UI into small, reusable presentational components

## Author

**Andrevis Jimenez** · Full Stack Developer
[Portfolio](https://andrevis.dev) · [LinkedIn](https://www.linkedin.com/in/andrevis-jimenez/) · [GitHub](https://github.com/Heiyey)
