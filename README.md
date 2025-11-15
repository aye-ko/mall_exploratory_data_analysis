# Customer Segmentation Analysis - Mall Customer Data

## Project Overview

**Objective:** Conduct exploratory data analysis on mall customer data to identify distinct customer segments and develop targeted marketing strategies to increase revenue.

**Key Results:**
- Identified 4 distinct customer segments using k-means clustering
- Statistical validation: Chi-square test confirmed segments have significantly different shopping preferences (p < 0.001)
- Developed a prioritized implementation plan targeting untapped high-value customer segments

**Skills Demonstrated:** R Programming | Statistical Analysis | K-Means Clustering | Hypothesis Testing | Data Visualization | Business Strategy

---

## Business Problem

**Goal:** Conduct exploratory data analysis and translate findings into actionable business insights.

**Audience:**
- Analytics team
- Business owner/stakeholders

**Ask:**
- What demographic spends the most?
- What category do they spend the most on?
- What strategies can increase sales across all customer segments?

**Business Task:** Identify high-value customer segments, understand their purchasing behavior, and recommend targeted strategies to increase revenue.

---

## Key Findings

The analysis revealed 4 distinct customer segments:

**1. Big Spenders (82 customers, 41%)**
- Middle-aged, loyal customers with high spending on luxury goods and electronics
- Highest current revenue contributors

**2. Efficient Spenders (36 customers, 18%)**
- Wealthy customers with high savings who only spend when necessary
- Untapped market with significant spending power

**3. Frugal Shoppers (54 customers, 27%)**
- Budget-conscious customers who are highly promotion-sensitive
- Frequent visitors with lower transaction sizes

**4. Poor-Young Spenders (28 customers, 14%)**
- Young customers with low income living above their means
- High spending despite limited resources, potential lifetime value

---

## Business Recommendations

**Priority 1: Efficient Spenders**
- Strategy: Reposition luxury items as "investment quality" purchases
- Messaging: "Buy once, use forever"
- Expected ROI: Highest potential - untapped market with spending power

**Priority 2: Big Spenders**
- Strategy: Expand VIP programs, exclusive early access to products
- Expected ROI: Highest reliability - proven spenders with strong loyalty

**Priority 3: Frugal Shoppers**
- Strategy: Sales events, BOGO offers, loyalty reward programs
- Expected ROI: Medium - frequent visits, lower ticket size

**Priority 4: Poor-Young Spenders**
- Strategy: Student discounts, ethical credit-building programs
- Expected ROI: Long-term lifetime value play
- Ethical Note: Avoid predatory lending practices

---

## Technical Approach

**Tools Used:**
- R Studio for data cleaning, analysis, and visualization
- R Markdown for reproducible reporting

**Analysis Steps:**

**1. Descriptive Statistics**
- Calculated mean, median, and standard deviation for all numeric variables
- Analyzed distribution shapes using skewness and kurtosis

**2. Relationship Analysis**
- Correlation analysis between customer characteristics and spending behavior
- Key finding: Loyalty years positively correlate with spending (r = 0.48)

**3. Customer Segmentation**
- Standardized all numeric features using z-scores
- Applied k-means clustering (k=4) to identify natural customer groups
- Validated segments with chi-square test of independence

**4. Statistical Validation**
- Chi-square test: X² = 140.24, df = 9, p < 0.001
- Confirms customer segments have significantly different shopping preferences

---

## Data Source

**Dataset:** Customer Analytics Practice Dataset  
**Source:** [Kaggle](https://www.kaggle.com/datasets/vikasjigupta786/customer-analytics-practice-dataset)

**Data Quality Assessment (ROCCC):**
- **Reliable:** Direct from mock company data
- **Original:** First-party company data
- **Comprehensive:** Contains all necessary variables for segmentation analysis
- **Current:** Static dataset (not real-time)
- **Cited:** Well-documented source

**Limitations:**
- The dataset contains 200 customers (relatively small sample)
- Data is not dynamic/real-time
- Limited to a point-in-time snapshot

---

## Project Files

- **Live Report:** [View Analysis](link-to-github-pages)
- **R Markdown:** [eda_report.Rmd]([link-to-file](https://github.com/aye-ko/mall_exploratory_data_analysis/blob/main/index.Rmd))
- **R Script:** [EDA.R](link-to-file)
- **Dataset:** [Mall_Customers_Enhanced.csv](https://www.kaggle.com/datasets/vikasjigupta786/customer-analytics-practice-dataset)

---

## How to Run This Analysis

**Prerequisites:**
```r
# Install required packages
install.packages(c("tidyverse", "ggplot2", "moments", "DT", "knitr"))
```

**Run the analysis:**
```r
# Load libraries
library(tidyverse)
library(ggplot2)
library(moments)
library(DT)

# Render the report
rmarkdown::render("eda_report.Rmd")
```

The analysis will generate an HTML report with all visualizations and findings.

---

## Data Cleaning Process

**Steps taken to ensure data integrity:**
1. Created a backup of the original raw data
2. Checked for and removed null values
3. Verified no duplicate customer records
4. Validated data types for all columns
5. Checked for spelling errors in categorical variables
6. Trimmed extra spaces from text fields

**Documentation:** All cleaning steps are documented in the R Markdown file with inline comments.

---

## Author

**Onyedikachukwu Okonkwo**  
Data Analyst 

---

## Acknowledgments

This project was completed as part of building a professional data analytics portfolio. Special thanks to the Kaggle community for providing practice datasets.
