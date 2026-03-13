# 2D Car Racing Game Specification

## Project Overview
- **Project name**: Night Rush
- **Type**: Browser-based 2D racing game
- **Core functionality**: Top-down arcade racing game where player dodges traffic and collects coins while racing against time
- **Target users**: Casual gamers

## UI/UX Specification

### Layout Structure
- Full-screen canvas game
- HUD overlay with score, speed, and time
- Start screen with title and instructions
- Game over screen with final score

### Visual Design
- **Color palette**:
  - Background road: #1a1a2e (dark asphalt)
  - Road lines: #f39c12 (yellow)
  - Grass/shoulder: #0f3d0f (dark green)
  - Player car: #e74c3c (red)
  - Enemy cars: #3498db, #9b59b6, #1abc9c (blue, purple, teal)
  - Coins: #f1c40f (gold)
  - HUD text: #ecf0f1 (white)
  - Accent: #e67e22 (orange)
  
- **Typography**:
  - Title: Bold, 48px
  - HUD: 20px monospace
  - Instructions: 16px

- **Visual effects**:
  - Road scrolling animation
  - Car shadow
  - Speed lines at high velocity
  - Explosion particles on collision
  - Coin sparkle effect

### Components
- Player car (rectangular with details)
- Enemy cars (varied colors)
- Road with lane markers
- Coins (rotating circles)
- HUD elements (score, speed, time)
- Start/Game Over overlays

## Functionality Specification

### Core Features
1. **Player controls**: Arrow keys or WASD for steering left/right, accelerate/brake
2. **Road scrolling**: Continuous vertical scroll with lane markings
3. **Enemy spawning**: Random enemy cars spawn at top, move down
4. **Coin collection**: Golden coins appear randomly, player collects for bonus points
5. **Collision detection**: Player collision with enemies ends game
6. **Scoring system**: Points for distance traveled + coin bonuses
7. **Speed increases**: Game gets progressively harder
8. **Lives system**: 3 lives, collision loses one life

### User Interactions
- Arrow Left/Right or A/D: Steer left/right
- Arrow Up/W: Accelerate
- Arrow Down/S: Brake
- Enter/Space: Start game / Restart after game over

### Game States
- START: Title screen with instructions
- PLAYING: Active gameplay
- GAME_OVER: Final score display with restart option

## Acceptance Criteria
1. Game starts with title screen showing controls
2. Player car responds to keyboard input smoothly
3. Road scrolls continuously creating illusion of movement
4. Enemy cars spawn and move down at varying speeds
5. Coins can be collected for bonus points
6. Collision with enemies reduces lives
7. Game ends when lives reach zero
8. Score displays correctly throughout gameplay
9. Game restarts properly after game over
