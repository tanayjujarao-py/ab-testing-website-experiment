# 📊 A/B Testing Analysis: Website Background Color Experiment

## Project Overview

This project presents an end-to-end A/B testing analysis to evaluate whether changing the website background color from **White (Control Group A)** to **Black (Treatment Group B)** improves user conversion.

Using statistical hypothesis testing, the analysis determines whether the observed increase in conversion rate is statistically significant while ensuring that user engagement metrics remain unaffected.

---

## Business Problem

An e-commerce company wanted to determine whether changing the website background color could improve user engagement and conversions.

The experiment aimed to answer the following questions:

- Does the new background color increase the conversion rate?
- Does it affect user engagement (time spent or page views)?
- Was the experiment properly randomized across different user segments?
- Should the new design be deployed?

---

## Dataset

The dataset contains approximately **5,000 user sessions** divided into:

- **Control Group (A)** – White background
- **Treatment Group (B)** – Black background

### Features

- User ID
- Group
- Page Views
- Time Spent
- Conversion
- Device
- Location

---

## Project Workflow

1. Data Loading and Inspection
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Conversion Rate Analysis
5. Two-Proportion Z-Test
6. 95% Confidence Interval
7. Welch's t-Test (Time Spent)
8. Welch's t-Test (Page Views)
9. Chi-Square Test (Device Distribution)
10. Chi-Square Test (Location Distribution)
11. Business Recommendation

---

## Statistical Methods Used

| Test | Purpose |
|-------|----------|
| Two-Proportion Z-Test | Compare conversion rates |
| 95% Confidence Interval | Estimate the true difference in conversion rates |
| Welch's t-Test | Compare average time spent |
| Welch's t-Test | Compare average page views |
| Chi-Square Test | Validate randomization across devices |
| Chi-Square Test | Validate randomization across locations |

---

## Key Results

### Conversion Rate

| Group | Conversion Rate |
|--------|----------------:|
| Control | **5.40%** |
| Treatment | **14.07%** |

- Statistically significant improvement
- 95% Confidence Interval excluded zero
- Null hypothesis rejected

---

### Time Spent

- No statistically significant difference between groups.

---

### Page Views

- No statistically significant difference between groups.

---

### Randomization Checks

Both Device and Location distributions were statistically similar across the Control and Treatment groups, indicating successful randomization.

---

## Business Recommendation

The treatment significantly improved the conversion rate without negatively affecting user engagement metrics such as page views and time spent.

Based on these findings, the new website background is recommended for deployment.

It is also recommended to continue monitoring conversion rate and guardrail metrics after deployment to ensure the observed improvement is sustained in a production environment.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Statsmodels
- Jupyter Notebook

---

## Project Structure

```
ab-testing-website-experiment/
│
├── data/
│   └── AB_Testing_Dataset.csv
│
├── notebooks/
│   └── AB_Testing_Analysis.ipynb
│
├── images/
│
├── README.md
├── requirements.txt
```

---

## How to Run

Clone the repository:

```bash
git clone https://github.com/tanayjujarao-py/ab-testing-website-experiment.git
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook and open:

```
notebooks/AB_Testing_Analysis.ipynb
```

---

## Skills Demonstrated

- A/B Testing
- Hypothesis Testing
- Statistical Inference
- Confidence Intervals
- Experimental Design
- Data Cleaning
- Exploratory Data Analysis
- Data Visualization
- Business Analytics
- Python for Data Analysis

---

## Key Takeaways

- Designed and analyzed an A/B experiment using industry-standard statistical methods.
- Interpreted statistical results in a business context.
- Distinguished between statistical significance and practical significance.
- Validated experiment randomization before making business recommendations.
- Produced an end-to-end analytical report suitable for product decision-making.

---

## Author

**Tanay Jujarao**

Aspiring Data Analyst passionate about statistics, experimentation, and data-driven decision making.
