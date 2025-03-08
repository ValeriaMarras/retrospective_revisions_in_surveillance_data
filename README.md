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
- [Configuration](#configuration)
- [License](#license)
- [Sources](#sources)

## Overview

The project is structured to handle two main aspects:
1. Analyzing retrospective corrections in surveillance data to quantify and characterize revisions.
2. Developing models to estimate data revisions for newly reported data to improve the quality of forecasting models.

## Prerequisites

- Python 3.7 or higher

## File Structure

- **dataset_generation.py**: Script to download and process snapshot data, and to generate a dataset with calculated revision metrics.
- **data_analysis.py**: Analyzes revision data, including calculating the frequency and magnitude of data revisions, and visualizing these trends.
- **forecasting_models.py**: Applies machine learning techniques to predict future revisions and integrates these predictions into forecasting models.

## Usage

### 1. Generating the Revision Dataset

Run `dataset_generation.py` to download snapshot files, calculate revision metrics like revision status and data age, and save the processed dataset.

### 2. Analyzing Revision Data

Execute `data_analysis.py` to load the generated dataset and perform statistical analysis on revision metrics, including plotting the revision magnitudes and probabilities.

### 3. Enhancing Forecasting Models

Use `forecasting_models.py` to apply the revision estimates from the machine learning models to improve the accuracy of short-term forecasting models.

## Configuration

Details how to configure the scripts to use different data sources or to filter data by specific dates or countries.

## License


## Sources

- Data is based on the [ERVISS surveillance system](https://erviss.org/).

By following these guidelines, users can effectively replicate and extend the analysis to accommodate new datasets or different infectious diseases.
