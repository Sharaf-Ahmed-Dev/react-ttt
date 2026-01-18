# Tic Tac Toe React App

A **Tic Tac Toe** game built using **React** and **Vite**.  
Two players can play alternately using X and O, with automatic win and draw detection, and a reset button to start a new game.

---

## Features

- Two-player gameplay (X and O)  
- Detects all winning combinations: 3 rows, 3 columns, 2 diagonals  
- Detects a draw when all squares are filled  
- Dynamic heading shows current status, winner, or draw message  
- New Game button resets the board  
- Uses images for X and O symbols  
- Prevents moves after a win or draw  

---

## How It Works

- The game board is represented by an array of 9 elements (`data = ["", "", "", "", "", "", "", "", ""]`).  
- **React hooks** used:  
  - `useState` for counting turns and locking the board  
  - `useRef` for accessing heading and box elements directly  
- **Toggle function** handles player moves:  
  - Adds X or O image to clicked box  
  - Updates the `data` array  
  - Increments move count  
  - Calls `checkWin` to see if the game has been won or drawn  
- **checkWin function** checks all possible win combinations and calls `won(winner)` if a player wins.  
- **won function** updates the heading with the winner and locks the board.  
- **draw function** updates the heading if all squares are filled without a winner.  
- **reset function** clears the board, resets the state, and unlocks the game for a new round.  

---


## Gameplay Instructions

1. Player X starts first.  
2. Click on an empty square to place X or O.  
3. Players alternate turns.  
4. When a player gets 3 symbols in a row (horizontally, vertically, or diagonally), they win.  
5. If all squares are filled without a winner, the game ends in a draw.  
6. Click the **New Game** button to restart.

---

## Technologies Used

- **React 18** – for building the UI and game logic  
- **JavaScript (ES6+)** – for handling game state and win/draw logic  
- **CSS3** – for styling the board, boxes, heading, and button  
- **Vite** – development build tool for fast setup  

---

## Live Demo

Try the game online here:  
[Play Tic Tac Toe](https://Sharaf-Ahmed-Dev.github.io/react-ttt/)

