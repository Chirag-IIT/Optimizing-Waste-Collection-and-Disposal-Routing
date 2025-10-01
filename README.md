# 🗑️ Optimizing Waste Collection & Disposal Routing

**Project Title:** Waste Collection & Disposal Routing Optimization  
**Domain:** Vehicle Routing / Waste Management / Operations Research  

---

## 📌 Overview  
Efficiently routing waste collection and disposal vehicles is critical for sustainable urban management. This project frames the problem as a Vehicle Routing Problem with Time Windows (VRP-TW) to minimize operational costs and improve service efficiency.

---

## 🎯 Objectives  
- Model the routing of collection and disposal vehicles under constraints (vehicle capacities, service time windows, route limits)  
- Generate routing solutions minimizing cost or distance  
- Compare algorithmic approaches (exact / heuristics)  
- Perform sensitivity analysis and visualize routing policies  

---

## 📁 Repository Structure & Files  

| File / Folder | Description |
|---------------|-------------|
| `Project Report.pdf` | Detailed problem statement, literature review, methodology, results |
| `Code for Problem.ipynb` | Main Jupyter notebook containing code, routing logic, and plots |
| `Delivery Nodes (Before Routing).png` | Map / scatter plot of delivery nodes prior to route planning |
| `Pickup Nodes (Before Routing).png` | Map / plot of pickup nodes before routing |
| `Vehicle Routes for Delivery CVRPTW .png` | Final routes for delivery side under CVRPTW formulation |
| `Vehicle Routes for Pickup CVRPTW.png` | Final pickup routing visualization |
| `Sensitivity Analysis: VRP.png` | Plot showing sensitivity of objective vs parameter variation |
| `README.md` | This descriptive file |

---

## 🧩 Problem Formulation & Approach  

1. **Data & Node Setup**  
   - Define pickup and disposal nodes (with coordinates, demand, service windows)  
   - Specify vehicle fleet capacity, available time windows, cost matrix  

2. **Mathematical Modeling**  
   - Variables: which vehicle visits which node, sequence order, time on arrival  
   - Constraints: capacity, time windows, flow conservation, route continuity  
   - Objective: minimize total cost/distance/time of routes  

3. **Solution Methods**  
   - Use Mixed Integer Programming (MIP) formulations (CVRPTW)  
   - Employ solver (e.g. Gurobi, CPLEX, or open-source solvers) for exact or near-optimal solutions  
   - Heuristic or metaheuristic enhancements (if needed) to scale  

4. **Visualization & Analysis**  
   - Map routes for delivery and pickup  
   - Compare against baseline (e.g., naive or greedy routing)  
   - Perform sensitivity analysis by varying capacities, time windows, node count  

---

## 📊 Key Results & Insights  
- The solver provided feasible routes that respect all pickup/disposal windows and vehicle limits  
- Route visualizations clearly show coverage across service zones  
- Sensitivity plots indicate how cost or distance responds to parameter changes  
- The approach demonstrates how OR + routing methods can significantly improve waste collection efficiency  

---

## 🚀 Future Extensions  
- Incorporate stochastic or dynamic arrival of waste (real-time demand)  
- Integrate more advanced heuristics (Tabu Search, Genetic Algorithms)  
- Scale to city-level routing with thousands of nodes  
- Add environmental constraints (emissions, fuel consumption)  

---

## 📸 Visualizations  

### Pickup Nodes (Before Routing)  
![Pickup Nodes](./Pickup%20Nodes%20(Before%20Routing).png)

### Vehicle Routes for Pickup CVRPTW  
![Vehicle Routes for Pickup CVRPTW](uploaded-image-2.png)

### Delivery Nodes (Before Routing)  
![Delivery Nodes](./Delivery%20Nodes%20(Before%20Routing).png)

### Vehicle Routes for Delivery CVRPTW
![Vehicle Routes for Delivery CVRPTW](uploaded-image-3.png)

### Sensitivity Analysis: VRP (Pickup and Delivery)
![Sensitivity Analysis VRP](uploaded-image-1.png)

---

## 📝 Usage Notes  
1. Install dependencies (e.g. `pandas`, `numpy`, solver API)  
2. Run `Code for Problem.ipynb` step by step  
3. Ensure image paths (in notebooks) point to the `*.png` files present  
4. Refer to **Project Report.pdf** for detailed derivations, model equations, and explanation  

---

## 👤 Author  
**Chirag Agarwal**  
[GitHub](https://github.com/Chirag-IIT) • [LinkedIn](https://www.linkedin.com/in/chirag-agarwal-iit)
