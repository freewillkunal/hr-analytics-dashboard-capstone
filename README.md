# Employee Performance & HR Analytics Dashboard

Capstone project for **Data Handling, Visualization & Feature Engineering (AML001)**.

**Name:** Kunal Pal | **Roll No:** 2601201042 | **BCA (H) AI & DS** | **Section B**

## Problem

An HR team wants to understand how **salary, experience and performance** relate across departments. This project builds an interactive Plotly dashboard that answers that question and states each finding in the chart titles.

## Repository contents

| File | Description |
|---|---|
| `HR_Analytics_Dashboard.ipynb` | Main notebook: dataset creation, inspection, correlation, groupby, dashboard, reflection |
| `HR_Analytics_Dashboard.html` | Exported interactive dashboard (download and open in a browser) |
| `sample_data_hr_employees.csv` | Sample dataset: 30 employees, 7 columns (created for this project) |
| `README.md` | This file |

**Exported outputs:** the interactive dashboard (`.html`). This project covers the exploratory analysis and dashboard stage of the workflow, so it does not train or export a machine-learning model.

## Execution steps

1. Open [Google Colab](https://colab.research.google.com) and choose **File → Upload notebook**.
2. Upload `HR_Analytics_Dashboard.ipynb`.
3. Choose **Runtime → Run all**. The first code cell installs Plotly and builds the dataset (no external file is needed; the same data is also in `sample_data_hr_employees.csv`).
4. The interactive dashboard appears in the Plotly cell: hover for values, drag to zoom, click the legend to hide or show departments.
5. The export cell saves `HR_Analytics_Dashboard.html`; the last cell downloads it (Colab only).

## What the notebook does

1. Creates a 30-record HR dataset (Department, Experience, Salary, Performance Score, Joining Date)
2. Inspects it with `shape`, `info()`, `describe()` and `value_counts()`
3. Calculates a correlation matrix and shows it as a heatmap
4. Runs a `groupby()` summary by department
5. Builds a 2x2 dashboard: scatter, bar, histogram and line chart, with finding-based titles and one fixed colour per department
6. Exports the dashboard as HTML
7. Ends with a written reflection

## Key findings

- Salary rises strongly with experience (correlation about 0.94)
- IT has the highest average salary and Operations the lowest
- 24 of 30 employees score between 2.5 and 4.0 on performance
- The dataset is small and was created for this exercise, so the findings should not be generalised

**Tools:** Python, Pandas, NumPy, Matplotlib, Plotly, Google Colab
