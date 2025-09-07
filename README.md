# Project Management Analytics

This project provides a **ready‑to‑use example** for business analysts, program managers and data analysts. It includes a synthetic dataset simulating project management scenarios, an exploratory analysis notebook with visualizations, and predictive models to demonstrate analytical techniques.

## Overview

The dataset contains 500 synthetic project records, each with metrics such as start and end dates, project duration, budget, team size, complexity, risk score and whether the project succeeded. The accompanying Jupyter notebook walks through the following:

* Loading and inspecting the dataset
* Visualizing distributions and relationships (histograms, scatter plots, bar charts and correlation heat map)
* Building a logistic regression model to predict project success
* Building a linear regression model to estimate project duration

The goal is to showcase how to perform data analysis and basic machine learning in a project management context.

## Files

| File | Description |
|---|---|
| `dataset.csv` | Synthetic project data used for analysis (500 rows). |
| `analysis.ipynb` | Jupyter notebook performing exploratory data analysis and predictive modeling. |
| `requirements.txt` | Python dependencies required to run the notebook. |
| `README.md` | This documentation. |

## Dataset description

The synthetic dataset includes the following fields:

| Column | Description |
|---|---|
| `project_id` | Unique identifier for each project. |
| `start_date` | Project start date. |
| `end_date` | Project end date, derived from the start date and duration. |
| `duration_days` | Length of the project in days. |
| `budget_k` | Budget allocated, in thousands of dollars. |
| `team_size` | Number of people working on the project. |
| `complexity_level` | Categorical measure of project complexity: **Low**, **Medium** or **High**. |
| `risk_score` | Numerical risk score from 1–9 (higher is riskier). |
| `vendor_count` | Number of external vendors involved. |
| `deliverables_count` | Number of deliverables the project must produce. |
| `success` | Binary indicator (1 for successful completion, 0 for failure). |

These values were generated using random distributions and simple logistic formulas to simulate real‑world variability.

## Installation

Ensure you have Python 3.8+ installed. Clone or download the repository, then install the required packages:

```bash
# Clone the repo (replace USERNAME with your GitHub username if using the web interface)
git clone https://github.com/<USERNAME>/project-management-analytics.git
cd project-management-analytics

# Create a virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt
```

## Usage

1. Open the Jupyter notebook:

   ```bash
   jupyter notebook analysis.ipynb
   ```

2. Run the notebook cells in order. The notebook will load `dataset.csv`, display summary statistics and generate several charts to help you explore the data.

3. The notebook then demonstrates two predictive models:
   * **Logistic Regression** predicting the likelihood of project success based on project metrics.
   * **Linear Regression** estimating project duration from budget, team size, risk score and other factors.

4. Feel free to modify the notebook or dataset to experiment with different scenarios, features or models.

## Customizing the dataset

The current dataset is synthetic and may not reflect your organisation’s real metrics. To generate a larger or different dataset, you can modify the data generation script (not included) or adjust values directly within the notebook. If you have real data, you can replace `dataset.csv` and re‑run the notebook.

## License

This project is provided for educational purposes. Feel free to adapt it for your own use.

## Notes

This repository was automatically generated as part of a job‑search portfolio. It includes a synthetic dataset and analysis notebook ready for use out of the box.

Feel free to fork this project and build upon it with your own datasets or further analysis techniques to showcase your skills as a business analyst, program manager or data analyst.
