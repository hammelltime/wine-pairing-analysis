# Wine Pairing Analysis

## Project Overview
Analysis of 34,000+ wine and food pairing combinations using SQL and Python to identify pairing patterns across wine types and food categories for sales recommendations.

## Tools Used
- Python (pandas, matplotlib, seaborn)
- SQL (SQLite)
- Jupyter Notebooks
- Data source: Kaggle

## Key Findings
- Cuisine types are evenly distributed
   - only 0.3% difference between least and most represented cuisines
- Food categories are not evenly distributed
    - 58.5% consist of red meat, cheese, and acidic
    - 41.5% comprised of remaining 9 categories
- Identified data limitations: data is synthetic/artificially balanced
    - Found uniformity among all 5 wine types paired with BBQ food
        - 3.0 average quality ratings
        - 255 pairings, evenly split by pairing quality rating (51 pairings rated 1, 51 pairings rated 2, etc.)

## Top average weighted quality ratings:
  - Tempranillo (3.15)
  - Chardonnay (3.11)
  - Zinfandel (3.10)
  - Syrah/Shiraz (3.10)
  - Cabernet Sauvignon (3.10)
  - Malbec (3.09)
  - Provence Rose (3.08)
  - Barbera (3.08)
  - Dry Riesling (3.07)

## Why Weighted Results?
- Weighted results provide a more balanced view of wine versatility across diverse food types, preventing over-representation of pairings like red meat
- Rankings shifted significantly from unweighted results, with Provence Rosé dropping out of top 5, suggesting it excels in specific categories rather than across all food types

## Retail implications
- Customers not pairing with a meal: recommend versatile wines with high weighted ratings
  - Opportunity to move slower inventory
- Customers pairing with a meal: see heat map for tailored suggestions

## Files
- `wine_analysis.ipynb` - Main analysis notebook with SQL queries and visualizations
- `data/wine_food_pairings.csv` - Dataset

## How to Run
1. Clone this repository
2. Open the Jupyter notebook
3. Run cells in order
