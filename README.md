# ILI and ARI Revisions Dataset and Analysis

This repository is dedicated to generating and analyzing Influenza-Like Illness (ILI) and Acute Respiratory Infection (ARI) data to improve forecast performance by anticipating data revisions.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [File Structure](#file-structure)
- [Usage](#usage)
  - [1. Generating the Revision Dataset](#1-generating-the-revision-dataset)
  - [2. Analyzing Revision Data](#2-analyzing-revision-data)
  - [3. Enhancing Forecasting Models](#3-enhancing-forecasting-models)
- [License](#license)
- [Sources](#sources)

## Overview

The project is structured to handle two main aspects:
1. Analyzing retrospective corrections in surveillance data to quantify and characterize revisions.
2. Developing models to estimate data revisions for newly reported data to improve the quality of forecasting models.

## Prerequisites

- Python 3.7 or higher

## File Structure

- **dataset_generation.ipynb**: Script to download and process snapshot data, and to generate a dataset with calculated revision metrics.
- **data_analysis.ipynb**: Analyzes revision data, including calculating the frequency and magnitude of data revisions, and visualizing these trends.
- **revisions_models.ipynb**: Applies machine learning techniques to predict future revisions.

## Usage

### 1. Generating the Revision Dataset

Run `dataset_generation.ipynb` to download snapshot files, calculate revision metrics like revision status and data age, and save the processed dataset.

### 2. Analyzing Revision Data

Execute `data_analysis.ipynb` to load the generated dataset and perform statistical analysis on revision metrics, including plotting the revision magnitudes and probabilities.

### 3. Revision Estimation Models

Use `revisions_models.ipynb` to estimate the new revisions from the machine learning models and baseline models.


## License


## Sources

- Data is based on the [ERVISS surveillance system](https://erviss.org/).

##

By following these guidelines, users can effectively replicate and extend the analysis to accommodate new datasets or different infectious diseases.
