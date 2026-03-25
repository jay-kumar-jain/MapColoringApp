# Map Coloring CSP

A high-performance, visual Constraint Satisfaction Problem (CSP) solver built with a Discord-inspired aesthetic. This tool demonstrates the **Four Color Theorem** and backtracking algorithms through an interactive graph interface.

🔗 Live Demo: [map-coloring-r2o8ajjyh-jaykumarjain012-7467s-projects.vercel.app](https://map-coloring-r2o8ajjyh-jaykumarjain012-7467s-projects.vercel.app/)

## 🎨 Features
- **Visual CSP Solver:** Watch the algorithm attempt to color nodes in real-time.
- **Backtracking Logic:** Implements a recursive search to ensure no two adjacent nodes share the same color.
- **Constraint Breach Detection:** Automatically identifies and alerts when a graph exceeds the 4-color theorem limits (non-planar cliques).
- **Glassmorphism UI:** Neon-accented, dark-mode interface with a soft-rounded workspace.
- **Interactive Nebula Intro:** Custom particle-warp animation on startup.

## 🛠️ Technical Stack
- **Frontend:** HTML5, CSS3 (Custom Variables & Animations).
- **Engine:** Vanilla JavaScript (ES6+).
- **Graphics:** HTML5 Canvas API for high-performance node rendering.

## 🧠 The Algorithm
The solver uses a **Backtracking Search** with the following constraints:
1. **Variable:** Each node on the canvas.
2. **Domain:** { Blurple, Magenta, Green, Yellow }.
3. **Constraint:** $Color(Node_A) \neq Color(Node_B)$ if an edge exists between $A$ and $B$.

If the graph is too dense (e.g., a $K_5$ complete graph), the solver will trigger a **Constraint Breach** notification after a 5-second computation safety timeout.

## 🚀 Quick Start
1. Clone the repository.
2. Open `index.html` in any modern web browser.
3. Click anywhere on the grid to create nodes.
4. Click one node and then another to create an edge.
5. Hit **Run Analysis**.

---
*Developed as a pedagogical tool for exploring Graph Theory and AI Logic.*
