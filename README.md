# Supplementary Material – Automated and explainable MCDA-based ERP pre-selection

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/myresearchbvp/ERP-MCDA-Simulation/blob/main/Automated_ERP_PreSelection.ipynb)

## 💡 About this repository
This repository contains the interactive simulator created for our study **"Automated and Explainable MCDA-based ERP Pre-Selection in Simulated Decision Scenarios"**. We uploaded this code so you can verify the results from the article, reproduce them on your own or simply see how the framework works in a real-world setting.

## ⚙️ What's inside?
The main file (`.ipynb`) is not just a block of code, but a fully interactive Decision Support System (DSS) dashboard that includes:

* **Data and scenarios** – we already pre-loaded the scores for the 4 ERP systems analyzed in the article, along with the weights for the three main strategic situations (Baseline, Feasibility, and Growth).
* **Consensus mode (S-Avg)** – a group decision-making feature that calculates the mathematical average of the predefined scenarios to simulate a democratic compromise between different stakeholders.
* **Advanced analytical metrics** – the system automatically computes several advanced MCDA (Multi-Criteria Decision Analysis) indicators:
  * *Efficiency to ideal solution (TOPSIS concept)* – measures how close the winning ERP is to absolute perfection.
  * *Head-to-head outranking (PROMETHEE/ELECTRE concept)* – evaluates direct pairwise performance and counts in how many criteria the winner directly beats the runner-up.
  * *Pareto dominance analysis* – checks if the recommended system mathematically dominates its rivals across all criteria.
  * *Gap analysis (goal seeking)* – calculates the exact raw performance improvement the runner-up needs to overturn the final ranking.
  * *Performance consistency* – a risk indicator based on the standard deviation of raw scores.
* **Automated explanation & stability tracking** – a rule-based module that translates complex math into plain text. It justifies the baseline winner by highlighting key weighted contributions, dynamically compares active scenarios against the baseline (S1), tracks scoring margins, and automatically identifies which criteria drove the observed changes.
* **Sensitivity analysis** – a dedicated one-click module that simulates a ±20% weight variation on the winner's most impactful criterion to mathematically test the robustness of the decision, outputting a dedicated threshold chart.
* **Dynamic visualization** – the ranking updates in real-time through a stacked bar chart, a radar chart for performance profiles, a donut chart for weight distribution, and a raw data heatmap.
* **Extended simulation and export** – you can go beyond the 4 examples in the text. You have the option to add up to 10 different systems, enter your own scores manually, and download your results instantly as comprehensive analytical reports (`.txt`), composite charts (`.png`), or raw data (`.csv`).

## 🚀 How to run the application
You don't need to install anything on your computer and you don't need any programming skills!

1. Click the **"Open in Colab"** badge at the top of the repository.
2. The code will open in a new Google Colab tab.
3. Go to the top menu, click **Runtime** and select **Run all** (or press `Ctrl+F9`).
4. Scroll to the bottom of the page where the interactive panel appears. 
5. Play with the sliders to change the importance of the criteria, load the ready-made scenarios, run the sensitivity analysis, or add your own data!

> ### 📝 Peer-review note
> We created this repository specifically for the review process. It is hosted on a generic account to respect the anonymity required by double-blind journal standards.
