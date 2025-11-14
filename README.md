# EvoNAS-Edge
# ResourceEvo: Edge-Aware Evolutionary Neural Architecture Search (EA-NAS)

**[Developed by a 16-Year-Old High School Student.]**

This project presents a **Multi-Objective Evolutionary Algorithm (EA-NAS)** system designed to solve the critical issues of large size and high latency in traditional ML models — especially for **Edge and IoT devices with constrained memory.**

The system autonomously discovers architectures that are **both more accurate AND VASTLY MORE EFFICIENT** than a manually designed, in-budget baseline model. This project demonstrates the practical viability of **Green AI** principles.

---

### 1. The Ultimate Fair Fight: Proof of Concept

The final test, conducted on the MNIST (10k subset) test set, proves that the AI-designed 'EA-Champion' model outperformed the human-designed, in-budget 32-bit baseline.

| Model | Acc(Test) | Latency (ms/sample) | Param(P) | Bit | Model Size (KB) | Budget Violation? |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Baseline (In-Budget, 60,) | **0.9425** | 0.0087 | 47710 | 32 | 186.37 | No |
| **EA-Champion (8-bit)** | **0.9470** | **0.0030** | 38965 | 8 | **38.05** | No |

### 2. Key Revolutionary Findings

* **Superior Accuracy:** The EA-Champion achieved **0.45% higher** test accuracy than the manually designed, budget-compliant baseline.
* **Efficiency Revolution:** The champion model is **~4.9x faster** and **~4.9x smaller** (38.05 KB vs. 186.37 KB footprint) than its fair competitor.
* **Technological Insight:** Model architectures optimized with **8-bit quantization awareness** are **ideal for constrained IoT/Edge devices** (Green AI principle).

### 3. Technologies & Methodology

* **Optimization:** NSGA-II (Non-dominated Sorting Genetic Algorithm II)
* **Search Objectives:** Maximize Accuracy, Minimize Cost (Parameter Count), and Minimize Latency (Proxy).
* **Frameworks:** Python, DEAP, Scikit-learn, NumPy.

### 4. How to Run the Experiment

The full evolutionary pipeline and analysis are available in the **`EvoNAS-Edge.ipynb`** file.

1.  Open the file in Google Colab.
2.  Select **Runtime → Run all**.

---
### 👤 Author & Contribution

**Author:** Mustafa Poyraz Çolak (16)

**Summary:** High School Student passionate about **Evolutionary AI**, **Edge-efficient Models**, and automated architecture search.

**Contribution:** Open to contributions — PRs and issues are welcome!
