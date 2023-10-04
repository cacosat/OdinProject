Assignment adapted from [The Odins Project Etch-a-Sketch Assignment](https://www.theodinproject.com/lessons/foundations-etch-a-sketch) into Conways Game of Life with the use of ChatGPT.

### 1. Set Up the Repository:
- Follow the same instructions provided in the assignment to set up a Git repository for the project.

### 2. Create the Grid:
- Create a webpage with a grid of square divs. The size of the grid (e.g., 16x16) will be configurable by the user.
- Use JavaScript to create the divs dynamically.
- Use flexbox or grid CSS to arrange the divs in a grid format.
- Each div represents a cell in Conway's Game of Life and can be in one of two states: alive (e.g., colored black) or dead (e.g., colored white).

### 3. Interact with Cells:
- Instead of a hover effect, set up a click event listener for each cell. When a cell is clicked, toggle its state between alive and dead.
- This allows the user to set the initial configuration of the grid by activating specific cells.

### 4. Implement Game Logic:
- Each cell looks at its eight neighbors and counts how many of them are alive.
- If a cell is alive:
  - It remains alive if it has 2 or 3 live neighbors; otherwise, it dies.
- If a cell is dead:
  - It becomes alive if it has exactly 3 live neighbors.
- Implement a function that applies these rules to each cell to produce the next generation.

### 5. Control Iterations:
- Add buttons to:
  - Start/pause the game: This will continuously apply the game logic to produce new generations.
  - Step forward: Apply the game logic once to produce the next generation.
  - Step backward: This is trickier as you'll need to store previous states of the grid. Consider using an array or another data structure to keep track of past configurations.
  - Reset: Clears the grid and allows the user to set a new initial configuration.

### 6. Configure Grid Size:
- Add a button that prompts the user to specify the grid size (e.g., 20x20).
- Once the size is entered, generate a new grid with the specified size. Ensure that the total space used remains constant, so the cells should adjust in size based on the grid dimensions.

### 7. (Optional) Enhancements:
- Add a counter to display the current generation number.
- Allow users to choose from predefined patterns or configurations (e.g., gliders, oscillators).
- Implement a speed slider to control how fast new generations are produced.

### 8. Push to GitHub:
- Once you've implemented and tested your Conway's Game of Life, push your project to GitHub.

