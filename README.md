# Optimizing-Conference-Carolinas-Travel-Using-Graph-Theory-and-Integer-Programming
This repository is from my research mathematics capstone class (Math 499) at Francis Marion University and was presented at the 2026 Francis Marion Undergraduate Mathematics Conference. It contains an optimized schedule model using Graph Theory &amp; Linear Programming to fix Conference Carolinas Women’s Soccer travel inefficiencies. Minimizes non-divisional mileage via integer optimization while keeping a strict round-robin structure. Includes the OpenSolver matrix dataset, presentation, etc.

# Optimizing Conference Carolinas Women’s Soccer Schedule Using Graph Theory and Linear Programming

**Researcher:** Tauzhanee Spann  
**Research Advisor:** Dr. Thomas Fitzkee  
**Institution:** Francis Marion University  

---

## 📌 Project Overview
This repository contains the optimization model, data structures, and research presentation with poster and powerpoint for overhauling the logistical inefficiencies in the Conference Carolinas Women’s Soccer scheduling system. 

By combining **Graph Theory** and **Linear Programming (Integer Optimization)**, this project builds a coordinated framework to minimize overall travel distances for non-divisional matchups while preserving a strict, balanced round-robin structure.

---

## 🛑 The Problem
In standard collegiate athletic scheduling, teams frequently travel separately and play on completely different days, which drastically increases operational costs and travel fatigue. 

While division games are locked, **non-divisional matchups** create an uneven scheduling problem because not all teams are required to play each other. This project targets those open slots to find the absolute most mileage-efficient matchups possible across the conference.

---

## 🧠 Methodology & Mathematical Models

### 1. Graph Theory Framework
* **Nodes (Vertices):** Each member institution in the Conference Carolinas represents a single node.
* **Weighted Edges:** The driving distances (mileage) between every school represent the weighted edges connecting those nodes.
* A comprehensive **Distance Matrix** was constructed to store these miles and serve as the foundation for the entire model.

### 2. Linear Programming & Integer Optimization
* **Decision Matrix:** A $16 \times 16$ binary matrix where a cell value of `1` indicates a scheduled non-divisional matchup and `0` indicates no game.
* **Objective Function:** Designed a matrix-based function to minimize the total conference travel distance:
  $$\text{Minimize } Z = \sum d_{ij}x_{ij}$$
* **Constraints:** Built mathematical boundaries ensuring that every team plays their designated number of non-division games without scheduling conflicts.
* **Algorithm:** Applied the **Branch and Bound** method to guarantee binary (whole number) scheduling solutions.

---

## 🛠️ Software & Tools Used
* **Advanced Excel / Google Sheets:** Used for data organization, distance matrix hosting, and constraint mapping.
* **OpenSolver:** Utilized this open-source linear programming extension because the sheer size of the $16 \times 16$ decision matrix and the volume of binary constraints completely exceeded the capacity of Excel's built-in Solver engine. 

---

## 📊 Results & Key Takeaways
* **Optimal Efficiency:** The model successfully solved the uneven scheduling problem, satisfying all competitive balance boundaries while establishing the shortest possible travel loops.
* **Impact:** Demonstrates how sports organizations and conference offices can leverage operations research tools to cut massive financial expenditures and reduce travel wear-and-tear on student-athletes.

---

## 🚀 Future Work
* Scaling the optimization script to coordinate schedules for all athletic sports programs at Francis Marion University.
* Incorporating Actuarial Science principles to model further cost-saving and predictive scheduling risk parameters.

---

## 🤝 Acknowledgements & References
* **Sponsor & Advisor:** Dr. Thomas Fitzkee
* **Course Support:** Mr. Phillips (Linear Programming)
* **Inspiration:** Savannah Bailey (Furman University) — *Linear Programming in ACC Women’s Basketball at NCUWM*

### Citations
* [Graph Theory Fundamentals for Beginners](https://www.numberanalytics.com/blog/graph-theory-fundamentals-beginners-guide)
* [Objective Function Concepts](https://www.cuemath.com/algebra/objective-function/)
* [Microsoft Solver Optimization Documentation](https://support.microsoft.com/en-us/office/define-and-solve-a-problem-by-using-solver-5d1a388f-079d-43ac-a7eb-f63e45925040)
* [Branch and Bound Algorithm - Wikipedia](https://en.wikipedia.org/wiki/Branch_and_bound)
* Powerpoint Presentation: [Spann_FMU.pptx](https://github.com/user-attachments/files/28607154/Spann_FMU.pptx) 
* Poster: [poster_fm_math (1).pptx] 
* Data:[FMU Women's Soccer.xlsx](https://github.com/user-attachments/files/28608302/FMU.Women.s.Soccer.xlsx)


