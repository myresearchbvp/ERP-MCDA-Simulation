# Supplementary Material: Automated and Explainable MCDA-based ERP Pre-Selection

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/myresearchbvp/ERP-MCDA-Simulation/blob/main/Automated_ERP_PreSelection.ipynb)

## About this Repository
This repository contains the interactive Python code used for the simulation study in our paper: *"Automated and Explainable MCDA-based ERP Pre-Selection in Simulated Decision Scenarios"*.

The code is provided as a supplementary resource to ensure transparency, reproducibility and to demonstrate the practical application of the proposed Decision Support System (DSS) framework.

## What's Inside?
The Jupyter Notebook (`.ipynb` file) includes the complete logic described in the paper:
* **Dataset & Weights:** The raw scores for the four anonymized ERP alternatives and the criteria weights for all three scenarios (Baseline, Feasibility-oriented, Growth-oriented).
* **MCDA Core Logic:** The weighted sum calculations used to determine the rankings and margins.
* **Visual Profiling:** Radar charts displaying the raw score profiles of the alternatives, and Stacked Bar charts showing exactly how each criterion contributes to the final score.
* **Automated Explanation:** A natural language generation (NLG) module that outputs clear, text-based justifications for the ranking results.
* **Interactive Dashboard:** A dynamic UI where you can adjust criteria weights via sliders and immediately see how the ranking and explanations change.

## How to Run the Code
You do not need to install Python or any libraries on your local machine.

1. Click the **"Open in Colab"** badge at the top of this page.
2. The code will open in a new Google Colab tab.
3. From the top menu, select **Runtime** > **Run all** (or press `Ctrl+F9`).
4. Scroll through the document to see the static results, and use the interactive dashboard at the very bottom to test different weighting scenarios.

## Peer-Review Note
This repository was created specifically for the peer-review process. It is maintained under a generic username to strictly preserve double-blind anonymity requirements.
