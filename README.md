# Educational Behaviors During COVID-19: Risk & Probabilistic Modeling

## 📌 Project Overview
Traditional machine learning models often struggle when handling highly interconnected, non-linear human behavior because they assume independent variables. During the shift to remote learning in the pandemic, student engagement was heavily dictated by a web of intertwined lifestyle disruptions (e.g., shifts in sleep schedules, stress levels, physical fitness, and screen time fatigue).

This project implements a **Bayesian Belief Network (BBN)** to map, quantify, and simulate how these behavioral variables dynamically influence one another. The resulting system allows stakeholders to calculate the exact probability of academic disengagement based on an individual student's changing daily habits.

## 🛠️ Tech Stack & Libraries
* **Language:** R (via RStudio / R Markdown)
* **Core Libraries:**
  * `bnlearn` - Used for structure learning (Hill-Climbing algorithm) and parameter estimation.
  * `Rgraphviz` - Deployed to visualize the Directed Acyclic Graph (DAG) layouts.
  * `tidyverse` & `ggplot2` - Implemented for data scrubbing, discretization, and descriptive data profiling.

## 🧠 Technical Methodology
1. **Data Preprocessing & Discretization:** Transformed continuous survey metrics into structured, discrete categorical state spaces (`Low`, `Medium`, `High`) to support non-linear probability maps.
2. **Structure Learning:** Built a **Directed Acyclic Graph (DAG)** by combining automated score-based algorithms with domain literature constraints to establish strict directional parent-child dependency layers.
3. **Parameter Estimation:** Calculated **Conditional Probability Tables (CPTs)** for every individual node to mathematically capture underlying behavioral dependencies across every possible permutation.
4. **Probabilistic Inference:** Configured conditional query engines (`cpquery`) to calculate predictive risk margins when fed hypothetical or partial student profiles.

## 📊 Key Insights Uncovered
* **The Fitness Buffer Effect:** Conditional inference queries revealed that physical activity acts as a structural statistical buffer. Students with high screen time who maintained high physical fitness had a significantly lower probability of academic disengagement compared to those with low physical activity.
* **Compounding Risk Cascades:** The model successfully proved that disengagement is rarely caused by a single isolated factor, but rather by cascading tipping points across multiple lifestyle habits.

## 📂 Repository Structure
* `/data` - Anonymized survey metadata profiles.
* `/scripts` - Source R scripts for structure mapping, parameter checking, and inference execution.
* `/plots` - Rgraphviz rendered visual DAG layouts.
* `README.md` - Technical documentation.
