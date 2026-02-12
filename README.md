# supply-chain-network-optimization 
*(Excel Analytic Solver Platform | Decision Analytics)*
# Supply Chain Network Optimization (Excel Analytic Solver Platform)

## Background
Designing an efficient supply chain network requires balancing transportation cost, capacity constraints, and market demand across multiple echelons.

This project addresses these objectives using **classification modeling** and **optimization-based decision analytics** implemented in Excel.

---

## Project Objectives
1. Identify which proposed suppliers should be approved for a new market.
2. Design a minimum-cost supply chain network connecting:
   **Suppliers → Ports → Distribution Centers**

---

## Tools & Methods
- **Excel Analytic Solver Platform**
- Classification Tree (Supplier Reliability)
- Mixed-Integer Linear Programming (MILP)
- Scenario and sensitivity analysis

---

## My Role
- Built a supplier reliability classification model using historical supplier data.
- Applied the model to evaluate and select potential new suppliers.
- Formulated and solved a MILP network optimization model in Excel.
- Analyzed optimization outputs and translated results into actionable recommendations.

---

## Methodology

### 1. Supplier Reliability Classification
- Trained a classification tree on 60 historical suppliers using six performance features:
  on-time delivery, lead time, defect rate, returns, unit cost, and cost variability.
- Applied the trained model to 15 proposed suppliers to predict reliability.
- Selected the **10 most reliable suppliers** for further network analysis.

**Key insight:**  
Defect rate is the primary driver of supplier reliability, followed by on-time delivery and cost stability.

---

### 2. Supply Chain Network Optimization
Using the selected suppliers, a **multi-echelon network** was optimized:

**Suppliers → Ports (Seattle, Los Angeles) → 26 Distribution Centers**

**Decision variables included:**
- Shipment quantities between suppliers, ports, and DCs
- Supplier usage decisions
- Optional supplier capacity upgrades

**Objective:**
Minimize total cost (transportation + capacity upgrade costs)

**Constraints:**
- 100% demand satisfaction at all DCs
- Supplier capacity limits with optional upgrades
- Minimum order quantity requirements
- Flow balance at ports

---

## Results

- **10 suppliers** were recommended based on reliability classification.
- **8 suppliers** were ultimately used in the optimized network.
- **4 suppliers** were upgraded, and all upgrades were fully utilized.
- Total optimized cost: **≈ $1.997M**
- Both Seattle and Los Angeles serve as major consolidation hubs.

The optimized network meets all demand while balancing cost efficiency and capacity investment.

---

## Recommendations
- Use defect rate as the primary screening criterion for future supplier evaluations.
- Maintain an approved supplier list and re-score suppliers as performance data updates.
- Rely on a core group of cost-effective suppliers with selective capacity upgrades.
- Periodically re-optimize the network as demand and transportation costs change.

---

## Notes
- Data and models have been simplified and anonymized for confidentiality.
- This project focuses on **decision analytics**, not software development.
