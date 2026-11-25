# Employee Burnout Prediction Analysis

**AI/ML Internship Project | Edunet Foundation | SRM University–AP | June–July 2024**

This repository contains the work completed for my eight-week Artificial Intelligence and Machine Learning internship conducted by **Edunet Foundation in collaboration with SRM University–AP**, leveraging the **IBM SkillsBuild** platform.

The project explores employee burnout patterns and applies **Linear Regression** to estimate employee burn rate using workplace and employee-related attributes.

## Project links

- **Repository:** https://github.com/abhiramreddy2603/EDUNET-Project-AIML
- **Jupyter Notebook:** [Internship_Project.ipynb](https://github.com/abhiramreddy2603/EDUNET-Project-AIML/blob/main/Internship_Project.ipynb)
- **View notebook (rendered):** [Open in nbviewer](https://nbviewer.org/github/abhiramreddy2603/EDUNET-Project-AIML/blob/main/Internship_Project.ipynb)
- **Dataset:** [employee_burnout_analysis-AI.xlsx](https://github.com/abhiramreddy2603/EDUNET-Project-AIML/blob/main/employee_burnout_analysis-AI.xlsx)

> **About deployment:** This repository contains a Jupyter Notebook and an Excel dataset, not a web application. There is no hosted interactive website to deploy. Use the notebook and rendered-notebook links above to explore the project.

## Project objective

Employee burnout can affect employee well-being and workplace productivity. The objective of this project was to explore factors associated with employee burnout and build a regression model to estimate **Burn Rate** from the available dataset.

## Dataset

The uploaded dataset contains **22,750 records and 9 columns** before preprocessing.

| Column | Description |
|---|---|
| `Employee ID` | Employee identifier |
| `Date of Joining` | Employee joining date |
| `Gender` | Employee gender |
| `Company Type` | Product or service company |
| `WFH Setup Available` | Whether a work-from-home setup is available |
| `Designation` | Designation level |
| `Resource Allocation` | Resource allocation value |
| `Mental Fatigue Score` | Mental fatigue score |
| `Burn Rate` | Target variable |

The notebook removes the employee identifier, encodes categorical values, checks missing values, and drops rows containing missing values. The resulting dataset contains **18,590 records**.

## Workflow in the notebook

1. Import Python libraries and load the Excel dataset.
2. Inspect the data using previews, descriptive statistics and dataset information.
3. Explore the relationship between Mental Fatigue Score and Burn Rate.
4. Check the correlation between those variables.
5. Remove the Employee ID column.
6. Encode categorical fields.
7. Inspect and remove rows with missing values.
8. Separate input features and the Burn Rate target.
9. Convert the joining-date field to a numeric representation.
10. Train a Linear Regression model.
11. Generate predictions and evaluate them using MAE and R².
12. Visualize actual and predicted values.

## Results recorded in the original notebook

The original notebook reports the following metrics after fitting and predicting on the same processed dataset:

| Metric | Recorded value |
|---|---:|
| Mean Absolute Error (MAE) | 0.05681 |
| R² score | 0.87300 |

**Evaluation note:** In the uploaded original notebook, the model is fitted and predictions are generated on the same data (`model.fit(inputs, target)` followed by `model.predict(inputs)`). These are therefore training-data metrics, not held-out test-set results. They should not be interpreted as evidence of performance on unseen data.

## Technologies used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- Microsoft Excel (`.xlsx` dataset)

## Run the notebook locally

1. Clone the repository:

   ```bash
   git clone https://github.com/abhiramreddy2603/EDUNET-Project-AIML.git
   cd EDUNET-Project-AIML
   ```

2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn plotly scikit-learn openpyxl jupyter
   ```

3. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `Internship_Project.ipynb`.

5. If running outside Google Colab, update the Excel file path in the notebook to the local dataset location.

## Internship details

- **Organization:** Edunet Foundation
- **Academic institution:** SRM University–AP
- **Learning platform:** IBM SkillsBuild
- **Domain:** Artificial Intelligence and Machine Learning
- **Duration:** 03 June 2024 – 31 July 2024 (8 weeks)
- **Project:** Employee Burnout Prediction Analysis

## Scope and limitations

This repository presents the notebook and dataset associated with the internship project. The work is an educational analysis using the supplied dataset. The notebook's original evaluation uses the same data for training and prediction, so a separate held-out evaluation would be needed to assess generalization to unseen records. The dataset's associations should not be interpreted as proof of causation or used as the sole basis for employment decisions.

---

*Completed as part of the Edunet Foundation AI/ML Summer Internship in collaboration with SRM University–AP and IBM SkillsBuild (2024).*
