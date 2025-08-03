# A-Data-Driven-Analysis-of-Household-Access-to-Basic-Services-in-Rwanda-DHS-2020-
# Household Access to Basic Services in Rwanda (DHS 2020)

## Project Overview
Analysis of electricity, water, sanitation, and internet disparities using Rwanda DHS 2020 data.

## Tools Used
- Python (Pandas for cleaning, Jupyter Notebook)
- Power BI (Visualizations)

## Dataset
[Download DHS 2020 Dataset](https://dhsprogram.com/data/Using-Datasets-for-Analysis.cfm)  
*Variables used*: electricity access, cooking fuel, water source, etc.

## Code Structure
- `rwanda_dhs_cleaning.ipynb`: Jupyter Notebook for data prep  
- `powerbi_dashboard.pbix`: Power BI file  

## How to Reproduce
1. Run the Jupyter Notebook to clean data  
2. Open Power BI file and refresh data source  

## Key Insights
- Urban households have 3× higher electricity access  
- Biomass fuel use correlates with thatch roofs (85%)

 ###Jupyter Notebook (Python)
Key Components to Includ

# Sample Code Snippets
import pandas as pd

# Load data
df = pd.read_csv('rwanda_dhs_2020.csv')

# Clean columns (example)
df['electricity_access'] = df['household has: electricity'].map({'Yes': 1, 'No': 0})

# Save cleaned data
df.to_csv('cleaned_rwanda_dhs.csv', index=False)
Notebook Sections:

Data loading

Column filtering (keep only relevant variables)

Missing value handling

Export to CSV for Power BI

###. Power BI Component
Files to Include:

powerbi_dashboard.pbix with:

4-5 key visuals (e.g., electricity vs. internet, water time poverty)

Interactive filters (residence type, roof material)

Consistent color scheme

Export Instructions:

In Power BI: File → Save As (ensure data source paths are relative)

Include a PDF/PPT export of the dashboard for backup.
###Dataset Link
Hosting: Upload cleaned data to GitHub or a cloud drive (Google Drive/Dropbox).

##README Note:
Data Source
[Rwanda DHS 2020](https://dhsprogram.com/data/Using-Datasets-for-Analysis.cfm)  
*Cleaned subset*: [Download here](your_cleaned_data_link)  
