# Environment

This supplementary tool was developed and tested in Google Colab.

## Recommended execution environment

- Google Colab
- Python 3.x
- Jupyter notebook interface
- Browser-based interactive widgets

## Main Python packages

The notebook uses the following packages:

- numpy
- pandas
- matplotlib
- ipywidgets
- IPython.display
- google.colab.files

The `google.colab.files` module is used for one-click file downloads from the Colab environment.

## Running in Google Colab

The recommended way to run the tool is to open the notebook directly in Google Colab and run all cells.

1. Open the repository on GitHub.
2. Click the **Open in Colab** badge from the README file.
3. In Colab, choose **Runtime > Run all**.
4. Scroll to the bottom of the notebook to use the interactive panel.

## Python script

The file `scripts/mcda_erp_preselection_tool.py` is a plain Python export of the notebook code. It is provided for inspection, reuse, adaptation.

Because the tool uses `ipywidgets`, `IPython.display` and `google.colab.files`, it is not intended as a standard command-line script. Advanced users may adapt it for local Jupyter execution, but the Google Colab notebook is the recommended route.

## Running locally

Local execution is possible in a Jupyter environment, but minor adjustments may be required for the download functions that use `google.colab.files`.

For the review process, Google Colab is the intended execution environment.