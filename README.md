# Memory-Puzzle-Game

This Memory Puzzle Game is a visual matching game designed using Python's tkinter library, with three difficulty levels: Easy, Medium, and Hard. The game challenges players to match hidden pairs of shapes or colors on a grid by flipping two cards at a time. Each card reveals a specific shape or color, and the objective is to match all pairs with the least number of moves.

# Libraries and Functions Used

Libraries

1. Tkinter: This library is used for building graphical user interfaces (GUIs) in Python. It provides a way to create windows, buttons, text inputs, and other graphical elements.

2. Canvas: Used to draw and manage objects like rectangles, ovals, and polygons on the window.

3. ttk: This is a submodule of Tkinter that provides themed widgets. It is used to create tabs for different difficulty levels.

4. Random: The random.shuffle function is used to randomize the positions of shapes on the board for each new game.

# Key Functions and Logic

1. draw(a, l, m):
This function is responsible for drawing the shapes on the canvas.
Based on the symbol (a), it creates different shapes (rectangles, ovals, and polygons) in various colors.

2. Parameters:
a: Character that defines which shape to draw.
l, m: Grid coordinates where the shape should be drawn.

3. quizboard():
It initializes the puzzle board by creating empty tiles and calling the draw function to show the shapes when necessary.
It also keeps track of how many shapes have been revealed.
If all tiles are revealed, it displays the total number of moves made by the player.

4. call(event):
This function is bound to the mouse click event on the canvas.
It determines which tile was clicked, checks whether a match has been found, and updates the board accordingly.
If a match is found, both tiles remain visible. Otherwise, the unmatched tiles are hidden again.

5. puzzleboard2() and call2(event):
These are similar to the quizboard() and call() functions but are designed for the Medium difficulty level with a larger grid and more shapes.

6. draw2():
This function is used in the Hard difficulty level and works similarly to draw(), but with a more extensive range of shapes and colors.

7. ttk.Notebook:
The Notebook widget creates multiple tabs, allowing the player to switch between different levels (Easy, Medium, and Hard).

8. random.shuffle:
The symbols that represent the shapes are shuffled randomly for each game, ensuring that the puzzle is different each time.
