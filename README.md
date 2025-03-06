# ILI Revisions Dataset and Analysis

A repository to generate and analyze ILI (Influenza-Like Illness) incidence data.  
This project contains two main Python scripts: one to generate a dataset with revision metrics and another to perform data analysis and visualization.

---

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [File Structure](#file-structure)
- [Usage](#usage)
  - [1. Generate the Dataset](#1-generate-the-dataset)
  - [2. Analyze the Data](#2-analyze-the-data)
- [Configuration](#configuration)
- [License](#license)

---

## Overview

This project is divided into two parts:

1. **Dataset Generation Script**  
   - Downloads snapshot files.
   - Loads the final reported data.
   - Processes the data for each country by:
     - Extracting dates from file names.
     - Calculating revision status (comparing snapshot values with final values).
     - Determining data age (in weeks, relative to the original report).
     - Computing the revision amount (difference between final and snapshot values).
     - Calculating the week in season.
   - Saves the final processed dataset as a CSV file in the `ILI_datasets` folder.

2. **Data Analysis and Visualization Script**  
   - Loads the generated dataset (or uses data directly from URLs).
   - Computes various revision metrics such as:
     - Number of revised data points per country.
     - ILI incidence plots for selected countries (snapshot reports and final data).
     - Error metrics (Error (E) and Percentage Error (PE)) via boxplots.
     - Revision probability by week (weeks after the original report).
     - Revision magnitude (average absolute change) per week.
   - Generates several plots to help visualize the analysis results.

---

## Prerequisites

- Python 3.7 or higher  
---

## File Structure

- **dataset_generation.py**  
  Retrieves snapshot files from a GitHub repository, loads snapshot and final reported data, processes the data to compute revision metrics, and saves the final dataset as a CSV file (`1_ILI_revisions_dataset_season_24_25_prova.csv`) in the `ILI_datasets` folder.

- **data_analysis.py**  
  Loads the generated dataset (or accesses the data from the URLs), computes various revision metrics (e.g., revised data points, error metrics, revision probabilities, and revision magnitudes), and generates multiple plots for visualization.

- **README.md**  
  This file.

---

## Configuration

- **URL Settings:**  
  Update the repository and URL settings in the scripts if data sources change.

- **Date Filtering:**  
  Both scripts filter data from a fixed starting date (e.g., October 2024). Adjust the filter as needed.

- **Country Selection:**  
  You can modify the list of selected countries (e.g., `['BE', 'DK', 'FR', 'NL', 'NO', 'IT']`) in the analysis script.


---

## License

---

By following these instructions, you should be able to generate the dataset and perform the analysis successfully.
