# 🤖 Intelligent Warehouse Robot Navigation

This project implements and compares multiple AI search algorithms for solving a constrained path-planning problem in a warehouse environment.

The goal is to guide a robot through a grid to collect maximum item value while respecting an energy constraint.

---

## 📌 Problem Overview

- The warehouse is modeled as an N × N grid
- The robot starts at (0, 0) and must reach (N-1, N-1)
- The grid contains:
  - Obstacles (blocked cells)
  - Items with weights (values)
- The robot has limited energy budget (E₀):
  - Each move costs 1 unit of energy

### 🎯 Objective

Maximize total collected weight W(π)

Subject to: L(π) ≤ E₀

---

## 🧠 Algorithms Implemented

### 🔹 Uninformed Search
- BFS (Breadth-First Search)
- UCS (Uniform Cost Search)

### 🔹 Informed Search
- Greedy Best-First Search
- A*
- Modified A* (Branch-and-Bound)

---

## 📏 Heuristics Used

- h1: Manhattan distance heuristic
- h2: Enhanced heuristic with MST and goal distance

---

## 🏗️ Project Structure

WarehouseRobot.ipynb
- Environment Definition
- Problem Generator
- Search Algorithms
- Heuristics
- Visualization
- Results

---

## ⚙️ Installation & Setup

pip install numpy matplotlib notebook

Run:
jupyter notebook WarehouseRobot.ipynb

---

## 📈 Key Insights

- BFS & UCS do not maximize reward
- Greedy is fast but suboptimal
- A* balances performance and efficiency
- Modified A* gives optimal reward

---

