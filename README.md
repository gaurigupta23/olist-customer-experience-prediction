# Olist Product Quality Analysis

This project analyzes the Olist Brazilian E-Commerce Public Dataset to identify drivers of poor customer experiences and recommend operational policies for category quality, logistics, listing standards, predictive intervention, and seller segmentation.

## Key Questions

- Which product categories carry the highest complaint risk?
- Are low reviews caused more by delivery failures or product defects?
- Does listing completeness affect customer satisfaction?
- Can low reviews be predicted before they are written?
- Can sellers be segmented into actionable quality groups?

## Main Deliverable

- `Olist_Analysis_Final.Rmd` is the final reproducible analysis report.
- The report reads all CSV files from the same folder, builds the analytical table, creates visualizations, trains a logistic regression model, and performs seller segmentation.

## Data

The analysis uses the Olist Brazilian E-Commerce Public Dataset from Kaggle:
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

All required CSV files are included in this repository for reproducibility.

## How To Run

1. Open `Olist_Analysis_Final.Rmd` in RStudio.
2. Make sure the working directory is the folder containing the Rmd and CSV files.
3. Install required packages if needed:

```r
install.packages(c(
  "tidyverse", "lubridate", "broom", "pROC",
  "knitr", "kableExtra", "scales", "patchwork", "rmarkdown"
))
```

4. Click **Knit** to generate the HTML report.

## Validation

The full report has been rendered successfully to `Olist_Analysis_Final.html`. The Rmd also includes a file-existence check so missing CSVs fail with a clear message before the analysis starts. 

🔗 **Live report:** https://gaurigupta23.github.io/olist-customer-experience-prediction/Olist_Analysis_Final.html
