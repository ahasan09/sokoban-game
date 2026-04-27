# Improvement Plan: sokoban_game

## Overview
Browser Sokoban game in vanilla JS. No multiple levels, no mobile support, no save state, and no undo functionality.

## Improvements

### Core Gameplay (High Priority)
- Add multiple levels — Sokoban traditionally has 50–100 levels; at minimum add 10
- Add an undo/redo system (store move history as a stack)
- Add a move counter and push counter displayed to the player
- Add level selection screen

### Level Format
- Store levels in a standard Sokoban level format (`.sok` or JSON) so levels can be added without modifying game code
- Import a free level pack (many are public domain) and include 20+ levels

### Mobile Support
- Add touch/swipe gesture controls
- Add on-screen directional buttons for mobile
- Ensure the game scales to fit different screen sizes (responsive canvas)

### Code Quality
- Separate game state (board, player position, history) from rendering logic
- Convert to TypeScript with a typed `GameState` interface
- Add ESLint + Prettier
- Add Jest unit tests for game logic (move validation, win condition detection, undo)

### Visual & UX
- Add smooth movement animation (tween the player and boxes)
- Add a solved/victory animation when a level is completed
- Add a "restart level" button
- Add localStorage-based progress saving (remember the highest solved level)

### DevOps
- Add Vite for bundling and dev server
- Add GitHub Actions CI: lint + test + build
- Deploy to GitHub Pages
