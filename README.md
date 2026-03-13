[อ่านภาษาไทยคลิกที่นี่](README_TH.md)
# GSL Engine
## Benchmark-Validated Deterministic Solver for Large-Scale CVRP
**High-Performance Routing Optimization for Industrial Logistics**

---

## Technical Overview
GSL Engine is a proprietary computational solver designed for the Capacitated Vehicle Routing Problem (CVRP). The system focuses on delivering stable, reproducible routing solutions for large-scale logistics environments.

Unlike stochastic metaheuristics, GSL is built on a structured deterministic heuristic framework. This guarantees consistent output across repeated executions—a critical requirement for industrial planning, auditing, and operational reliability.

The engine emphasizes:
* **Predictable Convergence:** Stable performance across diverse spatial distributions.
* **Scalable Computation:** Efficient handling of massive datasets without exponential latency.
* **Operational Practicality:** Designed for rapid decision-making in real-world logistics.

## Benchmark Validation: Set XL (2026)
The engine’s performance was evaluated on the complete **Set XL benchmark (100 instances)** introduced by **Queiroga et al. (2026)**, representing the current frontier of large-scale CVRP research.

* **Dataset Reference:** CVRPLIB – Extended Large-Scale Instances (Set XL)
* **Scope:** 100 / 100 Instances (Full Coverage)
* **Integrity:** 100% Feasibility (Zero-loss / All constraints strictly met)
* **Environment:** Standard CPU execution (Single-threaded)

### **Performance Matrix**
| Scale / Configuration | Observed Quality (Gap) | Typical Processing Time |
| :--- | :--- | :--- |
| **Mid-Scale (n=1,000)** | < 0.5% | 15 – 60 seconds |
| **Large-Scale (n=5,000)** | < 1.0% | 5 – 10 minutes |
| **Massive-Scale (n=10,001)** | **-0.06% (Match/Improve)** | ~18.6 minutes |
| **Complex Sparse Routes** | Verified Stability | Deep Refinement Capable |

## Observed Improvements over Recorded BKS (Snapshot)
The following results represent a performance snapshot compared against the Best Known Solutions (BKS) recorded in the CVRPLIB repository at the time of evaluation (March 2026).

| Instance | GSL Distance | Recorded BKS | Relative Difference |
| :--- | :--- | :--- | :--- |
| **XL-n1374-k278** | 232,139.97 | 233,049.00 | **-0.39%** |
| **XL-n10001-k1570** | 2,332,319.27 | 2,333,757.00 | **-0.06%** |

> ***Disclaimer:** BKS values in the Set XL benchmark are subject to ongoing improvements by the research community. These results are presented for comparative validation and do not claim permanent global optimality.*

## Potential Applications
The GSL Engine is optimized for:
* **Fleet Routing Optimization:** Minimizing fuel and operational costs.
* **Large-Scale Delivery Planning:** Managing complex urban distribution networks.
* **Supply Chain Logistics Modeling:** Strategizing multi-node transportation systems.
* **Industrial Distribution:** High-density customer cluster management.

## Operational Characteristics
* **Scalable Framework:** Maintains tractability on datasets exceeding 10,000 points.
* **Deterministic Logic:** Zero stochastic variance ensures auditable and reliable logistics planning.
* **High Throughput:** Engineered for environments requiring rapid re-routing or real-time updates.

## Professional Contact
**Independent Researcher: Chonmapoohm Thamsuwan (CTSuwan)** Email: ctsuwan@proton.me 
*Available for professional collaboration, routing optimization consulting, and large-scale logistics modeling services.*

**Service Platforms:**
* **Upwork**https://www.upwork.com/freelancers/~0173b4a58a1a327fd6?mp_source=share
* **Fastwork**

