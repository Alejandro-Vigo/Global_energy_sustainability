# Global ESG Trends: Energy, Economy & Environment

## Project Overview
This project analyzes global data to understand the complex interplay between economic development (GDP), environmental impact (CO2 emissions), and energy equity (access to electricity and clean cooking). Using a dataset covering 2000-2020, we explore whether countries can grow their economies without destroying the planet and how effective international aid is in driving sustainable development.

## Data Source
The dataset used in this analysis is sourced from Kaggle:
*   **[Global Data on Sustainable Energy (2000-2020)](https://www.kaggle.com/datasets/anshtanwar/global-data-on-sustainable-energy)**
    *   *Author:* Ansh Tanwar
    *   *Description:* A comprehensive dataset featuring sustainable energy indicators, including electricity access, renewable energy, and CO2 emissions for countries worldwide.

## Project Structure

The analysis is divided into a sequential workflow of Jupyter notebooks located in the `notebooks/` directory:

1.  **`00_Project_design.ipynb`**: Defines the analytical scope, Key Performance Indicators (KPIs), and "seed questions" that guide the investigation.
2.  **`01_Data_quality.ipynb`**: Initial data inspection, handling missing values, and validating data integrity.
    *   *Key Decision:* Structural missing values were preserved to avoid bias; specific missing metrics were flagged rather than aggressively imputed.
3.  **`02_Data_preparation.ipynb`**: Advanced cleaning, outlier detection, and feature engineering.
    *   *Key Decision:* Extreme values in GDP and CO2 were retained as they represent real-world global inequality, not data errors.
4.  **`03_EDA.ipynb`**: Exploratory Data Analysis answering the core seed questions through visualization and correlation analysis.
5.  **`04_Conclusions.ipynb`**: Summary of final insights and answers to the project's hypothesis.

## Key Findings

*   **The Decoupling Reality:** While GDP growth remains tightly linked to CO2 emissions globally, a small cluster of countries has successfully achieved "relative decoupling"—growing their economy while lowering emissions.
*   **Aid Effectiveness Paradox:** There is no strong statistical correlation between the volume of international financial aid received by a country and the speed of its subsequent electrification or renewable capacity growth. This suggests non-monetary barriers (infrastructure, policy, governance) are critical bottlenecks.
*   **The Infrastructure Lag:** Access to clean cooking fuels consistently lags behind access to electricity. Development tends to bring light before it brings clean air to the household kitchen.

## 📊 Interactive Dashboard (Tableau Public)

🔗 **View the interactive dashboard on Tableau Public:**  
https://public.tableau.com/views/TU_DASHBOARD

This dashboard explores the relationship between:
- Economic development
- CO₂ emissions
- Renewable energy
- Energy access and equity


## Installation

This project supports both Conda and Pip workflows.

### Option 1: Using Conda (Recommended)

1.  Clone the repository.
2.  Create and activate the environment:
    ```bash
    conda env create -f environment.yml
    conda activate esg
    ```

### Option 2: Using Pip

1.  Clone the repository.
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
