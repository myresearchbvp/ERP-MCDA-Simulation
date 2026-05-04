# Supplementary Material – A reproducible and explainable MCDA-based framework for ERP pre-selection in simulated decision scenarios

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/myresearchbvp/ERP-MCDA-Simulation/blob/main/notebooks/MCDA_ERP_PreSelection_Tool.ipynb)

## 💡 About this repository
This repository contains the interactive tool created for our study **"A reproducible and explainable MCDA-based framework for ERP pre-selection in simulated decision scenarios"**. We uploaded this code so you can verify the results from the article, reproduce them on your own or simply see how the framework works in an interactive simulated setting.

## 📁 Repository structure

```text
docs/
  ENVIRONMENT.md

notebooks/
  MCDA_ERP_PreSelection_Tool.ipynb

scripts/
  mcda_erp_preselection_tool.py

requirements.txt
README.md
LICENSE
```

The notebook is the main interactive version intended for Google Colab. The Python script is provided as a plain-code export for inspection, reuse and advanced execution in Colab or Jupyter-like environments. It is not designed as a command-line application.

## ⚙️ What's inside?
The main notebook (`.ipynb`) implements an interactive Decision Support System (DSS) dashboard that includes :

* **Data and scenarios** –> we already pre-loaded the scores for the 4 ERP alternatives analyzed in the article, along with the weights for the three main strategic situations (Baseline, Feasibility, Growth).
* **Consensus mode (S-Avg)** –> a group decision-making feature that calculates the mathematical average of the predefined scenarios to simulate a compromise weighting across different stakeholder priorities.
* **Advanced analytical metrics** –> the system automatically computes several advanced MCDA (Multi-Criteria Decision Analysis) indicators:
  * *Efficiency to ideal solution (TOPSIS concept)* – measures how close the winning ERP is to a hypothetical ideal alternative.
  * *Head-to-head outranking (PROMETHEE/ELECTRE concept)* – evaluates direct pairwise performance and counts in how many criteria the winner directly beats the runner-up.
  * *Pareto dominance analysis* – checks if the recommended system mathematically dominates its rivals across all criteria.
  * *Gap analysis (goal seeking)* – estimates the raw-score improvement the runner-up needs to overturn the final ranking.
  * *Performance consistency* – a risk indicator based on the standard deviation of raw scores.
* **Rule-based explanation & stability tracking** –> a rule-based module that converts numerical results into structured textual explanations. It justifies the baseline winner by highlighting key weighted contributions, dynamically compares active scenarios against the baseline (S1), tracks score margins and identifies which criteria contribute most to the observed changes.
* **Sensitivity analysis** –> a dedicated one-click module that simulates a ±20% weight variation on the winner's most impactful criterion to mathematically test the robustness of the decision, outputting a dedicated sensitivity chart.
* **Dynamic visualization** –> the ranking updates interactively through a stacked bar chart, a radar chart for performance profiles, a donut chart for weight distribution and a raw data heatmap.
* **Extended simulation and export** –> you can go beyond the 4 examples in the text. You have the option to add up to 10 different ERP alternatives, enter your own scores manually and download your results instantly as analytical text reports (`.txt`), composite charts (`.png`), raw data (`.csv`).

## 🚀 How to run the application
You don't need to install anything on your computer and you don't need any programming skills.

1. Click the **"Open in Colab"** badge at the top of the repository.
2. The code will open in a new Google Colab tab.
3. Go to the top menu, click **Runtime** and select **Run all** (or press `Ctrl+F9`).
4. Scroll to the bottom of the page where the interactive panel appears.
5. Play with the sliders to change the importance of the criteria, load the ready-made scenarios, run the sensitivity analysis or add your own data.

## 🧪 Python script
The file `scripts/mcda_erp_preselection_tool.py` contains a plain Python export of the notebook code. It is useful for code inspection, reuse, adaptation. Because the tool relies on interactive widgets, notebook display functions and Colab download functions, the recommended execution route remains the Colab notebook.

Advanced users may run or adapt the script in a Jupyter-like environment after installing the packages listed in `requirements.txt`. Local execution may require minor changes to the download functions that use `google.colab.files`.

## 🧩 Environment
The tool was developed for Google Colab. The main dependencies are listed in `requirements.txt`, and additional execution notes are provided in `docs/ENVIRONMENT.md`.

## 📝 Citation note
If you use this repository, please cite the associated manuscript once available.

> ### Peer-review note
> We created this repository for the review process.
