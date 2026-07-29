# Memory Game

A simple memory card matching game built with React and Vite. Flip cards to find matching pairs — complete all matches to win.

## Features

- Lightweight React + Vite app with HMR
- Component-based UI: `Card`, `GameHeader`, `WinMessage`
- Game logic encapsulated in `hooks/useGameLogic.js`

## Quick Setup

Prerequisites: Node.js 16+ and npm or Yarn.

Install dependencies:

```bash
npm install
# or
yarn
```

Start the development server:

```bash
npm run dev
# or
yarn dev
```

Build for production:

```bash
npm run build
# or
yarn build
```

Preview the production build locally:

```bash
npm run preview
# or
yarn preview
```

## How to Play

- Click a card to reveal it.
- Click a second card to try to match the first.
- Matching pairs remain revealed; non-matching pairs flip back.
- Match all pairs to see the win message.

## Project Structure (high level)

- `src/` — application source
  - `App.jsx`, `main.jsx`, `index.css`
  - `components/` — `Card.jsx`, `GameHeader.jsx`, `WinMessage.jsx`
  - `hooks/` — `useGameLogic.js`

## Contributing

Feel free to open issues or pull requests. Small, focused changes are easiest to review.

---

Enjoy the game!
