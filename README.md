A* Pathfinding Visualizer

This project is an interactive visualization of the A* (A-star) pathfinding algorithm using Pygame.
It allows users to draw a grid, set start and end nodes, add barriers, and watch the algorithm find the shortest path in real time.

🚀 Features

Interactive grid-based environment

Set Start and End nodes

Place Barriers (walls)

Visual animation of the A* search process

Final shortest path highlighted in Purple

Clear and restart options

Uses Manhattan distance heuristic for 4-directional movement

🎮 Controls
🖱️ Mouse Controls
Action	Behavior
Left Click (1st)	Set Start Node (Orange)
Left Click (2nd)	Set End Node (Turquoise)
Left Click (after that)	Place Barriers (Black)
Right Click	Reset any cell to empty
⌨️ Keyboard Controls
Key	Function
SPACE	Run the A* Algorithm (if start & end exist)
C	Clear the grid (entire board resets)
ESC / Window Close	Quit the program
🎨 Color Legend
Color	Meaning
White	Empty cell
Black	Barrier / Wall
Orange	Start Node
Turquoise	End Node
Green	In Open Set (to be explored)
Red	In Closed Set (already explored)
Purple	Final Path Found
🧠 How A* Works (In Simple Terms)

The algorithm tries to reach the goal using the formula:

f(n) = g(n) + h(n)


g(n): Cost from start → current node

h(n): Estimated cost from current → end (Manhattan distance)

f(n): Total predicted cost

A* always chooses the node with the smallest f(n) from the Priority Queue, making it very efficient and optimal.

🛠️ Setup & Installation
1️⃣ Install Python

Download Python 3.8+ from:
https://www.python.org/downloads/

2️⃣ Install Pygame

Run:

pip install pygame

3️⃣ Run the Program
python main.py

📁 Project Structure
├── main.py
├── README.md


main.py — Contains the A* logic and Pygame visualization

README.md — Documentation file

🧩 How the Code Works (Overview)
✔️ Spot Class

Represents each grid cell and handles:

drawing

color/state changes

neighbor detection

✔️ A* Algorithm

Implemented in the algorithm() function using:

PriorityQueue

g_score, f_score

came_from for reconstructing path

✔️ Real-time Visualization

The grid updates every frame to show:

open set

closed set

path

animations

⚡ Possible Improvements

Want to enhance it? Here are ideas:

Add diagonal movement

Weighted terrain (different movement costs)

Multiple algorithms (Dijkstra, BFS, Greedy BFS)

Speed control slider

Save/load grid maps

Maze generator (e.g., recursive backtracking)

📝 Author

Raghav Pasari
