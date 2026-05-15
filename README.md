# 🏓 Pong Game

A classic two-player Pong game built with Python's `turtle` graphics library.

## Gameplay

Two players compete by bouncing a ball back and forth using their paddles. If the ball passes a player's paddle, the opposing player scores a point. The ball speeds up slightly with each paddle hit, increasing the challenge over time.

## Controls

| Player | Move Up | Move Down |
|--------|---------|-----------|
| Left   | `W`     | `S`       |
| Right  | `↑`     | `↓`       |

## Project Structure

```
├── main.py         # Game loop, screen setup, collision detection
├── paddle.py       # Paddle class and movement logic
├── ball.py         # Ball class, movement, bouncing, and speed
└── scoreboard.py   # Scoreboard class, score tracking and display
```

## How It Works

- **Paddle** — Each paddle is a stretched square turtle that moves vertically in response to key presses.
- **Ball** — Moves diagonally and bounces off the top/bottom walls. On each paddle hit it reverses horizontal direction and speeds up by 10%.
- **Scoreboard** — Displays both scores at the top of the screen in large white text. Updates whenever a point is scored.
- **Collision detection** — The ball checks its distance from each paddle; a hit is registered when it's within 50 units and near the paddle's x-boundary.

## Requirements

- Python 3.x (no third-party packages needed — `turtle` is part of the standard library)

## Running the Game

```bash
python main.py
```

Click the window to exit after the game ends.
