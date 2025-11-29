# Claims Analysis

## Project Description
The project analyzes healthcare prospective claims data from May 202, with the intended goal of identifying common diagnoses/procedures, and understanding the payer mix to support compliance and revenue cycle operations. The analysis leverages Python - more specifically the pandas library to perform exploratory data analysis and aggregations, and the matplotlib and seaborn libraries to perform visualizations across the three interconnected claims datasets.

## Data Source Information
The analysis requires working with three interconnected, relational csv claims files: a HEADER file (claim-level information), a LINE file (service-level details and charges), and a CODE file (diagnosis and procedure codes). 

## How to Run the Notebook
1. Clone this repository in your local machine or google colab.
2. Ensure the three CSV files are in the same directory as the notebook or uploaded to your environment.
3. Open the Jupyter notebook or Google Colab notebook and run all cells sequentially from top to bottom.

## Summary of key findings
1. Based on the claim count, SB INTERNISTS is the top billing provider with 152 claims, followed by SB SURGICAL ASSOCIATES of 81 claims.
2. MEDICARE is the biggest primary payer, accounting for 71.0% of all claims, overwhelmingly more than the next highest payer, HEALTHFIRST FFS, which represents only 13.5% of claims.
3. The most common ICD-10 diagnosis code is J96.01 (Acute respiratory failure with hypoxia), with a frequency of 62, followed closely by I10 (Essential (primary) hypertension) and E78.5 (Hyperlipidemia, unspecified), both with a frequency of 49.
4. HCPCS code 99291 (CRITICAL CARE, INITIAL FIRST HOUR) is the most frequently billed procedure, occurring 68 times, substantially more often than the next highest codes, 99233 and 99233, which both occur 48 times.
5. Ambulatory Surgery claims exhibit the highest average charge ($1912.50), significantly exceeding other facility locations, while Outpatient Hospital claims report the lowest average charge ($330.43).

## Required Libraries
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```