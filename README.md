# Python-Snake-Game-
A polished Snake game built with Python’s Tkinter. Features real-time score and persistent high score, pause/resume, restart, “start from beginning” (resets high score), dynamic emoji obstacles, and bonus food every 10 points. 

# Python Snake Game – Tkinter GUI

A classic Snake Game implemented in Python with a Tkinter GUI, score & high‑score tracking, pause/resume, restart, dynamic obstacles, and occasional bonus food.

## Features
- Smooth movement on a grid with arrow keys
- **Score** and **High Score** persisted to `snake_high_score.json`
- **Pause/Resume**, **Restart**, **Start from Beginning** (resets high score), and **Exit**
- Random **obstacles** (with emojis) that spawn over time
- **Bonus food** worth +2 every 10 points
- Walls appear automatically at higher scores to increase difficulty
- Motivational messages that rotate every few seconds

## Requirements
- Python 3.8+ (works on Windows/macOS/Linux)
- Standard library only (`tkinter`, `json`, `random`, `os`)

## Run
```bash
python snake_game.py
```

## Controls
- **Arrow keys**: move snake
- **Pause** button: pause/resume
- **Restart**: restart round (keeps high score)
- **Start from Beginning**: reset high score to 0 and start
- **Esc**: quit

## Notes
- All timers are safely cancelled at game over.
- Bonus food appears exactly at multiples of 10 (fixed operator precedence bug).
- Walls are validated before drawing to avoid invisible/overlapping "ghost" walls.

