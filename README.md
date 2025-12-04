# Graph Explorer Toolkit

An educational Visual Basic .NET application that allows users to build graphs, run algorithms, and observe each step through animated visuals.  
Designed for classrooms, demonstrations, and self-learning.

---

## 📘 Project Summary

Graph Explorer Toolkit provides an interactive workspace where learners can draw graphs, connect nodes, assign weights, and watch classical graph-theory algorithms unfold visually.  
This tool aims to make algorithmic behaviour easier to understand by turning abstract theory into clear animations.

---

## 🚀 Key Capabilities

### 🧩 Graph Editing Interface
- Create nodes labeled A–Z  
- Draw weighted or unweighted edges  
- Rearrange nodes freely on the canvas  
- Choose between:
  - **Manual Weight Mode** – type in custom weights  
  - **Auto-Distance Mode** – weights computed from node spacing  

### 🔍 Algorithm Visual Walkthroughs
The toolkit supports detailed, step-by-step visualizations of:

#### Traversal & Routing
- **Breadth-First Search (BFS)**  
- **Depth-First Search (DFS)**  
- **Dijkstra’s Shortest Path Algorithm**

#### Optimization
- **Travelling Salesperson Route Exploration**
  - Full permutation search for small graphs  
  - Greedy nearest-neighbor estimation for larger ones  

### 🎨 Visualization Features
- Real-time color transitions for visited, active, and completed nodes  
- Animated edge highlighting  
- Adjustable playback speed slider  
- Automatically updated graph representations  

---

## 🗂 Graph Data Views
- **Adjacency Matrix** – grid representation of all connections  
- **Adjacency List** – compact mapping of neighbors  
Both views sync automatically whenever the graph changes.

---

## 💾 Saving & Loading Graphs
- Store graphs to XML files  
- Load previously saved configurations  
- Restore a prebuilt demonstration graph  
- Clear or rebuild the workspace any time  

---

## 🛠 Internal Architecture

### Core Components
- `GraphModel` – manages nodes and edges  
- `VertexControl` – interactive node UI  
- `EdgeLink` – drawable weighted connection  
- Basic `Queue` and `Stack` structures for algorithm operations  

### Algorithm Modules
- `RouteFinderDijkstra`  
- `TraverseBFS`  
- `TraverseDFS`  
- `TSPSolverBruteforce`  
- `TSPSolverGreedy`  

### Serialization Objects
- `GraphState`  
- `NodeState`  
- `EdgeState`  

These allow exporting and importing the full graph structure.

---

## 🧭 How to Use

### Start Quickly
1. Open the program to load the sample graph  
2. Add or remove nodes as needed  
3. Drag nodes to reposition them  
4. Right-click on nodes to create edges  

### Build Your Own Graph
1. Click **Add Node**  
2. Choose a node label  
3. Connect nodes through the context menu  
4. Pick a weight mode  
5. Inspect adjacency list/matrix to verify structure  

### Run an Algorithm
1. Select start/target nodes  
2. Choose an algorithm from the menu  
3. Adjust the animation slider  
4. Watch visual steps and final results  

### Additional Tools
- Generate a fully connected graph (distance-mode only)  
- Save & reload graph layouts  

---

## 🎓 Who Should Use This?

- Students learning graph theory  
- Teachers needing visual demos  
- Programmers exploring algorithm behavior  
- Anyone curious about routing, traversal, or graph optimization  

---

## 🖥 System Requirements
- Windows OS  
- .NET Framework  
- Visual Basic .NET (Windows Forms)

A preview C# port using **Avalonia UI** is included in the `Cross-platform/` directory for Linux/macOS/Windows users.

---

## 📊 Complexity Overview
| Algorithm | Complexity | Notes |
|----------|------------|-------|
| BFS / DFS | O(V + E) | Linear graph traversal |
| Dijkstra | O(V²) or O(E + V log V) | Depends on data structure |
| TSP (Brute Force) | O(n!) | Enumerates all tours |
| TSP (Greedy) | ~O(n²) | Fast heuristic |

---

## 📜 License
This project is intended for educational use. Modify or extend as needed.
