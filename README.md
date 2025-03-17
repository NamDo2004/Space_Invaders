# Space Invaders - Pygame
## Overview
This is a classic Space Invaders game implemented in Python using the Pygame library. Players control a spaceship to defend against waves of enemy ships by shooting lasers while avoiding enemy attacks. The game features increasing difficulty, a health bar, and lives tracking.

## Features
- Player-controlled spaceship with movement and shooting capabilities.
- Enemy ships with random spawning and laser attacks.
- Collision detection between ships and lasers.
- Health bar for the player and lives counter.
- Level progression with increasing enemy waves.
- Game over screen when lives or health run out.

## How It Works
### Classes
1. **Laser**: Represents laser projectiles with movement, collision detection, and off-screen removal.
2. **Ship**: Base class for all ships, handling drawing, laser movement, and shooting cooldown.
3. **Player**: Inherits from Ship. Controls the yellow spaceship with WASD keys and spacebar for shooting. Includes a health bar.
4. **Enemy**: Inherits from Ship. Randomly spawns red, green, or blue enemy ships that move downward and shoot lasers.

## Game Mechanics
- **Player**: Moves left (A), right (D), up (W), down (S), and shoots (SPACE). Health decreases on enemy -collision or laser hits.
- **Enemies**: Spawn in waves, move downward, and shoot randomly. Removed when hit by player lasers or when they pass the screen (costs a life).
- **Levels**: Each wave cleared increases the level and spawns more enemies.
- **Game Over**: Triggered when lives reach 0 or player health depletes, displaying "You lost!!!" for 3 seconds before closing.

## Requirements
- Python 3.x
- Pygame library (pip install pygame)
- Assets folder with images (ships, lasers, background) located at ```/Space_Invaders.py/assets/assets```

## Setup
1. Ensure Python and Pygame are installed.
2. Place the script in a directory with the assets folder containing:
- pixel_ship_red_small.png, pixel_ship_green_small.png, pixel_ship_blue_small.png (enemy ships)
- pixel_ship_yellow.png (player ship)
- pixel_laser_red.png, pixel_laser_green.png, pixel_laser_blue.png, pixel_laser_yellow.png (lasers)
- background-black.png (background)
3. Update file paths in the script if your assets are stored elsewhere.
