# 📊 Process Mining with Real-World Financial Loan Applications

Welcome to a comprehensive analysis of a **real-world banking loan application process**, powered by **process mining techniques** and data-driven insights. This project investigates event logs from a Dutch bank to explore efficiency, compliance, bottlenecks, and performance using advanced analytical and process discovery tools.

---

## 📁 Project Description

This repository presents the full pipeline of **process mining** applied to a **financial loan application system**. Utilizing a real **event log with over 262,000 entries across 13,087 loan cases**, this project offers:

* Deep insights into operational inefficiencies and rework loops
* Process model discovery and validation
* Resource usage assessment and improvement recommendations

---

## 🎯 Objectives

* 🔍 Analyze structural and temporal aspects of loan processing workflows
* 🛠 Handle and impute **missing data** from the event log
* ⏱ Visualize process **duration, frequency, and transitions**
* ♻️ Identify **rework loops** and process **variants**
* 👷 Evaluate the **efficiency of resource utilization**
* 🧭 Apply **process discovery algorithms** to uncover actual workflows
* 🚀 Recommend process enhancements to mitigate inefficiencies

---

🖼️ Process Visualizations
Below are visualizations of the discovered process models using different process mining techniques:

🔷 Heuristics Miner
![image](https://github.com/user-attachments/assets/30f7307b-1407-4022-bb15-edbfb08b0d24)

🔷 Alpha Algorithm 
![image](https://github.com/user-attachments/assets/81f49c54-3974-48c6-af25-901dbb8b2406)

🔷 Inductive Miner 
![image](https://github.com/user-attachments/assets/785716a2-2a7a-4f96-b402-4c79f6989802)

---

## 🔎 Dataset Overview

* **Source:** Real bank event logs (2012, The Netherlands)
* **Volume:** 262,200+ events across 13,087 loan cases
* **Fields Included:**

  * `Case_ID` — Unique identifier for each loan request
  * `Activity` — Executed process activity
  * `Timestamp` — Time of activity (start, complete, schedule)
  * `Resource` — Responsible person/system
  * `Amount_Request` — Loan amount requested

---

## ⚙️ Methods & Tools

### 🔧 Process Mining Techniques

* **Discovery Algorithms:**

  * Heuristics Miner (DFG & Petri Net)
  * Alpha Miner
  * Inductive Miner (BPMN)

* **Conformance Checking:**

  * Token Replay
  * Alignments
  * Evaluation Metrics: *Fitness*, *Precision*, *Generalization*, *Simplicity*

---

### 📊 Analytical Techniques

* Event log cleaning and preprocessing
* Missing value handling using **mode-based imputation**
* Process decision tree construction
* Variant and transition frequency analysis
* Productivity heatmaps of resources
* Throughput time evaluation and visualizations

---

### 🧰 Tools & Libraries

* Python 3
* `pandas`, `pm4py`, `scikit-learn`, `seaborn`, `matplotlib`
* Jupyter Notebooks for reproducible analysis

---

## 💡 Key Findings

* 🔀 Over **50 unique process variants** detected
* 🔁 Frequent **rework patterns** found in manual tasks
* ⛔ Identification of **bottlenecks** in human-involved activities
* 🔧 **Redundant tasks** merged to streamline the process
* 📈 Optimized performance by focusing on **top 12 process variants**, covering \~50% of all cases
