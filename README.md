# Customer Churn Analysis and Customer Intelligence

**Author:** Karan Ambhore  
**Project Type:** Data Analytics / Exploratory Data Analysis (EDA)  
**Primary Language:** Python

## 1. Project Overview

This project explores customer data to understand customer behavior and identify patterns that may be associated with customer churn. It demonstrates a practical data analytics workflow, including data import, data cleaning, feature engineering, SQL integration, exploratory analysis, and visualization.

The current project is an analytics and EDA project. It does not claim to train or deploy a machine-learning churn prediction model unless that functionality is added separately.

## 2. Objectives

- Load customer data from Excel, CSV, and a SQLite database.
- Inspect tables, columns, and data types.
- Clean and standardize data for analysis.
- Handle missing values and prepare useful analytical features.
- Combine related data tables using joins where appropriate.
- Explore trends and relationships in the customer data.
- Create visualizations with Matplotlib and Seaborn.
- Communicate findings that may help a business investigate customer retention.

## 3. Technologies and Libraries

- **Python** — core programming language
- **Pandas** — data loading, cleaning, transformation, and analysis
- **NumPy** — numerical operations
- **Matplotlib** — charts and plots
- **Seaborn** — statistical visualizations
- **SQLite / sqlite3** — local relational database and SQL queries
- **Jupyter Notebook** — interactive analysis
- **OpenPyXL** — Excel `.xlsx` file support for Pandas

## 4. Project Structure

```text
Data Analytics Python Project/
├── churn_analysis.ipynb          # Main analysis notebook
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

> The notebook may create or replace tables in `customer_churn.db` when the database setup cell is run. Keep a backup if you need to preserve an existing database.
>
> Customer datasets and generated database files are kept local and are not included in this repository. Obtain the source workbook from an authorized source and place it beside the notebook before running the analysis.

## 5. Installation

### Prerequisites

- Python 3.10 or later recommended
- pip
- Jupyter Notebook

### Set up a virtual environment (recommended)

**Windows PowerShell:**

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## 6. How to Run

1. Download or clone the project folder.
2. Keep the notebook and its input files in the same project directory, unless you update the file paths in the notebook.
3. Install the dependencies using `requirements.txt`.
4. Start Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open `churn_analysis.ipynb`.
6. Run the cells from top to bottom. Review the database setup notes in the notebook before recreating the SQLite database.
7. Review the generated tables, data-cleaning steps, analyses, and plots.

## 7. Analysis Workflow

1. **Data import:** Read Excel sheets and/or load tables from SQLite into Pandas DataFrames.
2. **Data inspection:** Review table names, columns, and data types.
3. **Data cleaning:** Rename columns, remove unnecessary fields where justified, correct data types, standardize values, and handle missing data.
4. **Feature engineering:** Create useful derived columns and join related datasets where appropriate.
5. **Exploratory analysis:** Summarize the data and investigate customer patterns.
6. **Visualization:** Use Matplotlib and Seaborn to present findings.
7. **Export:** Save prepared data for reuse where needed.
8. **SQL practice:** Demonstrate basic SQLite table creation and querying in Python.

## 8. Dataset and Data Notes

The notebook expects `customer_churn_data_raw.xlsx` in the project directory and creates or uses `customer_churn.db`; it can also export `exported_churn_data.csv`. These files may contain customer data and are intentionally excluded from version control. Obtain and use the source workbook only when authorized.

Before publishing this project, document the actual source of the data, its license, the meaning of important columns, and whether the data contains personal or confidential information. Do not upload sensitive customer data without permission.

## 9. Expected Deliverables

- A Jupyter notebook documenting the analysis process
- Cleaned and transformed customer data
- Exploratory summaries and visualizations
- SQL/SQLite data handling examples
- Exported data where appropriate
- Project documentation and dependency list

## 10. Business Value

Customer churn analysis can help a business investigate which customer groups may need attention, understand customer behavior, and develop questions for retention strategies. Conclusions should be based on the actual data and visualizations; this README does not assume specific findings or model accuracy.

## 11. Future Improvements

- Add a clearly documented churn-rate KPI and other business metrics.
- Create an interactive Power BI dashboard.
- Add a machine-learning churn prediction pipeline with a train/test split and suitable evaluation metrics, if prediction is part of the project scope.
- Compare model performance using precision, recall, F1-score, and ROC-AUC, especially if churn classes are imbalanced.
- Add tests, data validation, and a reproducible environment file with pinned dependency versions.

## 12. Author

**Karan Ambhore**  
B.E. Information Technology Graduate  
Interests: Python, Data Analytics, SQL, Data Visualization, and Machine Learning

---

*Created for learning, portfolio development, and demonstration of data analytics skills.*
