# Sokoban Game

A browser-based implementation of the classic [Sokoban](https://en.wikipedia.org/wiki/Sokoban) puzzle game. Push boxes (`B`) onto all goal cells (`O`) to complete each level.

## How to Play

- Use **Arrow Keys** to move the player
- Push boxes (`B`) onto goal spots (`O`)
- All goals must be covered to win
- Reload the page to reset the puzzle

## Map Legend

| Symbol | Meaning |
|--------|---------|
| `W` | Wall |
| `B` | Box |
| `O` | Goal spot |
| `X` | Box on goal |
| `S` / player | Player position |
| (space) | Open floor |

## Running

No installation needed. Open `index.html` directly in any modern browser:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

Or serve locally:

```bash
npx serve .
```

Then open [http://localhost:3000](http://localhost:3000).

## Prerequisites

- Any modern web browser (Chrome, Firefox, Edge, Safari)

## Project Structure

```
sokoban-game/
├── index.html   # Entry point
├── index.js     # Game logic — map rendering, box pushing, win detection
├── style.css    # Grid and cell styles
└── assets/      # Game assets
```
