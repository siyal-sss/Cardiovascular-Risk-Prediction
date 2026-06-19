 # Cardiovascular Risk Prediction

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/siyal-sss/Cardiovascular-Risk-Prediction/blob/main/Project_1.ipynb)

This repository contains a machine learning workflow focused on predicting cardiovascular risks based on medical records and patient data. The goal is to analyze specific clinical indicators and accurately identify whether a patient tests positive or negative for cardiovascular disease risk.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Specifications](#dataset-specifications)
- [Project Structure & Workflow](#project-structure--workflow)
- [Prerequisites & Dependencies](#prerequisites--dependencies)
- [Getting Started](#getting-started)
- [Visualizations Produced](#visualizations-produced)

---

## Project Overview
Cardiovascular diseases are one of the leading causes of health complications globally. Early identification of clinical traits can facilitate early intervention. This project leverages a data-driven approach to clean, analyze, visualize, and build prediction workflows using a dataset of clinical medical features. 

## Dataset Specifications
The pipeline expects a structured dataset file named `Medicaldataset.csv`. It contains **1,319 instances** across the following clinical indicators:

* **Age**: Age of the patient (ranging from 14 to 103 years)
* **Gender**: Categorized marker (Binary: `0` or `1`)
* **Heart rate**: Patient beats per minute
* **Systolic blood pressure**: Peak arterial pressure during cardiac contraction
* **Diastolic blood pressure**: Minimum arterial pressure during cardiac relaxation
* **Blood sugar**: Glucose concentration
* **CK-MB**: Creatine Kinase-MB enzyme levels (cardiac biomarker)
* **Troponin**: Troponin protein levels (key regulatory protein for cardiac muscle injury diagnosis)
* **Result**: The target prediction column (`positive` or `negative`)

The dataset does not contain missing null values, and the target distribution contains **810 positive instances** and **509 negative instances**.

## Project Structure & Workflow
The analysis is structured inside `Project_1.ipynb` following standard data science pipelines:

1.  **Data Loading & Inspection**: Uses `pandas` to read the medical records dataset, checking dataset structure, features, datatypes, and integrity checks via `.info()`, `.describe()`, and `.isnull().sum()`.
2.  **Exploratory Data Analysis (EDA)**: Investigates target balance and outcomes.
3.  **Data Visualization**: Uses `matplotlib` to plot and export target class distributions (`cardiovascular_outcome_distribution.png`).
4.  *(Optional expansion points: Feature preprocessing, model selection, and model metric analysis such as evaluation via ROC Curves).*

## Prerequisites & Dependencies
The code is written in Python 3. To run this project locally, ensure you have the following packages installed:

* `pandas`
* `matplotlib`

You can install these dependencies using `pip`:
```bash
pip install pandas matplotlib
