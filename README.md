# Pong Game Web Application

A modern web-based Pong game with leaderboard, multiplayer, and analytics support, built with Node.js, Express, and Socket.io.

## Features

- Play Pong against AI or another player (W/S and Arrow keys)
- Real-time multiplayer over the network
- Leaderboard for top scores
- Game history and analytics
- Modern UI with player profiles

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or newer recommended)

### Installation

1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Install dependencies:
   ```
   npm install
   ```

### Running the Application

1. Start the backend server (serves both API and frontend):
   ```
   npm start
   ```
2. Open your browser and go to [http://localhost:4001](http://localhost:4001)

## Controls

- **Right Paddle:** Arrow Up / Arrow Down
- **Left Paddle (Manual):** W / S
- **Left Paddle (AI):** Select AI in the start form

## API Endpoints

- `GET /api/leaderboard` — Get top scores
- `POST /api/score` — Submit a score (`{ player, score }`)
- `GET /api/history` — Get recent game history
- `POST /api/history` — Submit a game result (`{ players, scores, winner }`)

## Multiplayer

- Two players can join from different browsers/devices.
- The server pairs players automatically for real-time play.

## Project Structure

- `public/` — Frontend files (HTML, CSS, JS)
- `server.js` — Node.js backend (API, WebSocket, static serving)

## License

MIT
