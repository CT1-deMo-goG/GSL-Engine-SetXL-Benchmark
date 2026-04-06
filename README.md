[อ่านภาษาไทยคลิกที่นี่](README_TH.md)
# GSL Engine: Set XL Hyper-Scale Portfolio
**Deterministic Optimization for Ultra-Large CVRP (1,000 - 10,000 Nodes)**

## Technical Overview
GSL Engine is a proprietary computational solver designed for the Capacitated Vehicle Routing Problem (CVRP). The system focuses on delivering stable, reproducible, and **Real-time** routing solutions for large-scale logistics environments. 

Unlike stochastic metaheuristics, GSL is built on a structured deterministic framework, ensuring consistent output across repeated executions—a critical requirement for industrial planning and operational reliability.

---

## 📊 Benchmark Validation: Set XL (2026)
Evaluated on the complete Set XL benchmark (100 instances), representing the current frontier of large-scale CVRP research.

### Performance Summary
* **Massive-Scale (n=10,001):** **-0.06% Gap** (Matched/Improved BKS)
* **Typical Processing Time:** ~5.40s (at 10,000 nodes)
* **Win Rate vs LNS (300 Iter):** 98%+ (At this scale, metaheuristics face "Iteration Breakdown")
* **Integrity:** 100% Feasibility (Zero-loss)

### Observed Improvements over Recorded BKS
* **XL-n1374-k278:** **-0.39% Gap**
* **XL-n10001-k1570:** **-0.06% Gap**
* **XL-n2028-k617:** **-0.08% Gap**

---

## 🔍 Operational Scope & Characteristics

### **Strengths**
* **Scalable Framework:** Maintains tractability and **Real-time** speed on datasets exceeding 10,000 points.
* **Deterministic Logic:** Zero stochastic variance ensures auditable and reliable logistics planning.
* **High-Density Performance:** Optimal for urban logistics where many vehicles ($k$) are deployed.

### **Operational Constraints (Limitations)**
* **Low-Density / Low $k$ Scenarios:** GSL is optimized for high-density clustering. In cases where the number of vehicles is very small relative to the number of nodes (**Low $k$ / High $n$**), a higher gap compared to the mathematical optimum may be observed.
* **Complex Sparse Routes:** While stable, sparse networks with extreme distances between nodes are better suited for deep refinement solvers if execution time is not a critical constraint.

---

## 📂 Repository Structure
* **[Solution Files](./):** Verified `.sol` files for all hyper-scale instances located in the root directory.
* **[Benchmarks](./Benchmarks):** Detailed scalability analysis, comparative baseline data (GSL vs. CW vs. LNS), and full execution logs.

---

## Professional Contact
**Independent Researcher:** Chonmapoohm Thamsuwan (CTSuwan)  
**Email:** [ctsuwan@proton.me](mailto:ctsuwan@proton.me)  
**Platforms:** [Upwork Profile](https://www.upwork.com/freelancers/~0187428f64582f3473)


