# Hyper-Scale Performance Report: Set XL (1,000 - 10,000 Nodes)

This folder documents the performance of GSL Engine V22 in hyper-scale environments, compared against **Clarke-Wright (CW)** and **LNS**.

## ⚙️ Benchmarking Methodology & Environment
At hyper-scale, computational endurance and time-to-solution are the key metrics.

* **Environment:** Mobile-native processing (Snapdragon/Android).
* **LNS Constraint:** Bounded to **300 iterations**. At the 10,000-node scale, stochastic metaheuristics (LNS) face significant **"iteration breakdown,"** as they cannot sufficiently explore the massive search space within a **Real-time** window.
* **Deterministic Advantage:** GSL Engine V22 relies on structured decomposition, maintaining consistency even when search-based methods fail to converge within the same time constraints.

## 🚀 Hyper-Scale Benchmark Table
Performance results for 1,000 to 10,000-node instances.

| Instance | BKS | GSL Gap | CW Gap | LNS Gap (300 Iter) | Winner |
| :--- | :--- | :--- | :--- | :--- | :--- |
| XL-n10001-k1570 | 2333757.0 | **-0.06%** | 3.66% | 67.75% | **GSL** |
| XL-n1374-k278 | 233049.0 | **-0.39%** | 4.82% | 73.53% | **GSL** |
| XL-n2028-k617 | 544403.0 | **-0.08%** | 6.50% | 39.14% | **GSL** |
| XL-n2354-k631 | 940825.0 | **-0.22%** | 6.03% | 35.24% | **GSL** |
| XL-n5288-k1246 | 1960101.0 | **-0.17%** | 5.32% | 47.42% | **GSL** |

## ⚡ Scalability Insights
* **10,000 Nodes:** GSL successfully identifies solutions with negative gaps in **Real-time**, demonstrating its edge over metaheuristics that struggle with complexity.
* **Efficiency:** Maintains stability in large-scale logistics networks where traditional heuristics (CW) start to show increased gaps.
* **Deterministic Stability:** The structured logic ensures that solution quality remains robust as node counts increase.
* 
