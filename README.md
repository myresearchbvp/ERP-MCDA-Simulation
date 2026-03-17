# Supplementary Material – Automated and Explainable MCDA-based ERP Pre-Selection

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/myresearchbvp/ERP-MCDA-Simulation/blob/main/Automated_ERP_PreSelection.ipynb)

## About this Repository
This repository contains the interactive simulator created for our study – **"Automated and Explainable MCDA-based ERP Pre-Selection in Simulated Decision Scenarios"**. We uploaded this code so you can verify the results from the article, reproduce them on your own, or see how the system works in a real-world setting.

## What's inside
The main file (`.ipynb`) is not just a block of code, but an interactive dashboard that includes –

* **Data and scenarios** – We already loaded the scores for the 4 ERP systems from the article and the weights for the three analyzed situations (Balanced, Feasibility, or Growth)
* **Calculation logic** – Everything related to the math behind the rankings and margins
* **Dynamic charts** – The ranking changes before your eyes through a bar chart that shows exactly how much each criterion mattered for the final score
* **Automated explanations** – A module that translates numbers into text and explains clearly why a certain system came out on top
* **Extended simulation** – You can go beyond the 4 examples in the text; you have the option to add up to 10 different systems and even enter your own scores manually to see the outcome

## How to run the application
You don't need to install anything on your computer and you don't need programming skills.

1. Click the **"Open in Colab"** badge above
2. The page will open in a new Google Colab tab
3. Go to the top menu, click **Runtime** and select **Run all** (or press `Ctrl+F9`)
4. Scroll to the bottom of the page where the interactive panel appeared. Play with the sliders to change the importance of the criteria, load the ready-made scenarios, or add your own data

> ### Peer-Review Note
> This repository was created specifically for the review process. It is hosted on a generic account to respect the anonymity required by journal standards.
