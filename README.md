# A-Data-Driven-Analysis-of-Household-Access-to-Basic-Services-in-Rwanda-DHS-2020-
1. Why this topic?
Because it focuses on core living conditions that affect millions of people — and it's measurable using clear, structured data.

DHS 2020 includes key indicators like:

Access to electricity

Source of drinking water

Type of toilet facilities

Residence type (urban vs rural)

Household wealth level

Regional differences (province)

As a Big Data & IT student, this topic lets you apply:

Data cleaning

Categorical analysis

Visualization (Power BI or Python)

Possibly even prediction/classification

And you get to do that in a way that produces insights anyone can understand.

 2. Importance of the Topic
 Why does it matter?
These basic services are part of Sustainable Development Goals (SDGs), especially:

SDG 6: Clean Water and Sanitation

SDG 7: Affordable and Clean Energy

Understanding these gaps helps governments, NGOs, and policymakers make smarter decisions

It exposes inequality — showing which areas or groups are left behind
💬 Example:
If your data shows that rural Western Province has low electricity access, that’s a signal for targeted investment.
| Challenge                                 | How to Overcome It                                         |
| ----------------------------------------- | ---------------------------------------------------------- |
| DHS dataset is large and complex          | Focus only on a few key variables (electricity, water)     |
| Data is coded numerically (e.g., 1 = Yes) | Use the DHS codebook to decode variables                   |
| Missing or inconsistent data              | Use Python or Power BI to filter, clean, and impute        |
| Urban-rural or regional imbalance in data | Use grouping and percentage analysis instead of raw counts |

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

