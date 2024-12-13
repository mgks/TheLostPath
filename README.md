# The Lost Path

Step into the ever-changing labyrinths of The Lost Path, a 2D maze adventure crafted with HTML5 Canvas. Collect treasures, navigate twists, and race against the clock to escape!

## Gameplay

In The Lost Path, players navigate a procedurally generated maze using the arrow keys. The objective is to reach the blue finish point (the end of the maze) from the top-left corner before the timer runs out.

## Features in Version 1.0

*   **Procedurally Generated Maze:** Each game generates a new random maze using a recursive backtracking algorithm, ensuring a unique experience on every playthrough.
*   **Keyboard Controls:** Players use the arrow keys (Up, Down, Left, Right) to move through the maze.
*   **Centered Player:** The player character remains centered on the screen, and the maze shifts around them, providing a focused view of the immediate surroundings.
*   **Timer:** A countdown timer adds a sense of urgency. The timer starts when the player makes the first move. The initial time is calculated based on 5 seconds per tile on the shortest path to the finish (determined using Breadth-First Search).
*   **Restart Functionality:** Players can restart the game at any time using the "Restart" button. A new maze is generated upon restart.
*   **Win Condition:** When the player reaches the finish, a "Congratulations!" message is displayed, and the game automatically restarts after 3 seconds.
*   **Game Over Condition:** If the timer runs out, a "Time's Up!" message is displayed and the game restarts after 5 seconds.
*   **Debug Mode:** When enabled, displays all possible paths, turning the maze into white instead of black, making it easier to navigate. Activated by pressing `Shift + D`.
*   **Cheat Detection:** The game detects when the player wins with debug mode on, and displays a different message.

## Technical Details

*   **HTML5 Canvas:** The game is rendered on an HTML5 `<canvas>` element, providing a flexible and efficient way to draw graphics and animations.
*   **JavaScript:** The game logic, maze generation, rendering, and event handling are all implemented in JavaScript.
*   **Maze Generation:** The maze is generated using a recursive backtracking algorithm. This algorithm starts at a given cell, randomly moves to an unvisited neighbor, and continues until all cells are visited, carving out paths in the process.
*   **Pathfinding (for Timer):** A Breadth-First Search (BFS) algorithm is used to find the shortest path from the player's starting position to the finish. This path is used to calculate the initial timer value.
*   **Collision Detection:** The game checks for collisions between the player and the maze walls. The player cannot move through walls.
*   **Timer Implementation:** The timer is implemented using `requestAnimationFrame` for smooth updates and accurate timing.

## Development Roadmap

### Version 1.0 (Current Release)

*   **Status:** Completed
*   **Focus:** Core gameplay mechanics, basic UI.
*   **Features:**
    *   Keyboard-controlled player movement.
    *   Centered player with maze shifting.
    *   Procedurally generated maze.
    *   Timer with dynamic initial time calculation.
    *   Restart button.
    *   Win and Game Over conditions.

### Version 2.0 (Planned)

*   **Focus:** Gameplay enhancements, new features, and improved visuals.
*   **Features:**
    *   **Collectibles:** Add collectible items within the maze.
    *   **Stats Board:** Display collectibles gathered and other relevant information.
    *   **Background Music:** Add looping background music.
    *   **Advanced Maze Generation:** Implement more sophisticated maze generation algorithms (e.g., Kruskal's, Prim's).
    *   **Enemies:** Add enemies with basic AI.
    *   **Player Torch:** Implement a visual "torch" effect.
    *   **Menu/Options:** Add a main menu with game options.
    *   **Touch/Mouse Controls:** Implement touch controls for mobile devices and mouse dragging for desktop.
    *   **Responsive Design:** Adapt to various screen sizes.

### Version 3.0 (Future)

*   **Focus:** Character development, enhanced visuals, and storytelling elements.
*   **Features:**
    *   **Level Management:** Introduce multiple levels with increasing difficulty.
    *   **New Maze Styles:** Explore different maze layouts (e.g., circular, hexagonal).
    *   Character Design and Animation
    *   Enemy AI Enhancements
    *   Player Powers
    *   Dungeon Atmosphere

## Installation

No installation is required. Simply open the `index.html` file in a web browser to play the game.

## Contributing

Contributions to The Lost Path are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Submit a pull request, clearly describing your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

I'm not a game developer and this experimental project is a collaborative effort, co-created with insights from various LLMs, online resources, and the valuable contributions of current and future contributors.

## Closing Note

***For new developers:** Programming can be challenging at times, but with practice and persistence, you can develop the skills to create amazing things. The beauty of programming is that it empowers you to bring your ideas to life and create your own world. Keep exploring & experimenting. All the best for your next project!*

[![Profile](https://forthebadge.com/images/badges/built-with-love.svg)](https://mgks.dev)
