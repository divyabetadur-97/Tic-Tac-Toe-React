# Tic Tac Toe React Game

A two-player Tic Tac Toe game built with React, featuring player name customization, game history tracking, and winner detection.

## Features

- **Two-Player Gameplay** - Play as Player 1 (X) and Player 2 (O)
- **Player Name Customization** - Edit player names during the game
- **Game History** - View all moves
- **Winner Detection** - Automatic detection of winning combinations
- **Draw Detection** - Identifies when the game ends in a draw
- **Reset Game** - Restart the game
- **Responsive UI** - Clean, interactive interface

## React Concepts Used

### 1. Functional Components
- All components are built as function-based React components for modern, clean code

### 2. Hooks
- `useState` - Manages player names, game turns, and UI state (editing mode)

### 3. Props & Component Composition
- Modular component structure with data passed through props
- Components: `Player`, `GameBoard`, `Log`, `GameOver`

### 4. Event Handling
- Click handlers for board moves and button actions
- Input change handlers for player name editing
- Conditional button disabling based on game state

### 5. List Rendering
- Dynamic rendering of the 3×3 game board using `.map()`
- Rendering game history logs dynamically

### 6. State Lifting
- Central state management in `App.jsx`
- Game state (`gameTurns`, `players`) passed down to child components

### 7. Conditional Rendering
- Display different UI based on game state (active player, winner, draw)
- Toggle between display and edit modes for player names
- Show game over screen only when game ends

### 8. Derived State
- Computing values from base state without storing redundant data
- Functions: `deriveActivePlayer()`, `deriveGameBoard()`, `deriveWinner()`
- Calculated values: `activePlayer`, `gameBoard`, `winner`, `hasDraw`

### 9. Controlled Components
- Input fields for player names controlled by React state
- Button states controlled by component logic

### 10. Immutability & State Updates
- Using spread operators (`...`) to create new state objects and arrays
- Functional state updates with `setGameTurns(prevTurns => ...)`
- Preserving original state while creating new versions


## Getting Started

### Prerequisites
- Node.js 
- npm 

### Installation

```bash
# Install dependencies
npm install

Development
# Start the development server
npm run dev
