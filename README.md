# GIST-Data-Science-Internship-
# GIST Data Science Internship — Task 1
## Data Cleaning & Exploration

This project completes **GIST Data Science Task 1**, which requires data cleaning, missing-value handling, duplicate removal, outlier identification, descriptive statistics, and basic visualizations.

### Dataset
**Student Performance Factors**  
Source: Kaggle — https://www.kaggle.com/datasets/lainguyn123/student-performance-factors

The dataset contains student study habits, attendance, parental/school factors, lifestyle variables, and `Exam_Score`.

### Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

### Project workflow
1. Load the dataset
2. Inspect structure and data types
3. Measure missing values
4. Handle missing numeric values with median imputation
5. Handle missing categorical values with mode imputation
6. Detect and remove duplicate records
7. Calculate descriptive statistics
8. Detect potential outliers using the IQR method
9. Visualize exam-score distribution
10. Analyze study hours and attendance against exam scores
11. Generate a numeric correlation matrix
12. Explore categorical factors
13. Validate final dataset quality
14. Export the cleaned dataset

### Files
- `GIST_Task1_Data_Cleaning_Exploration.ipynb` — complete Colab notebook
- `README.md` — project documentation
- `data/` — cleaned dataset after running the notebook

### How to run
1. Open the notebook in Google Colab.
2. Run cells from top to bottom.
3. The notebook downloads the public Kaggle dataset using `kagglehub`.
4. At the end, download `student_performance_cleaned.csv`.
5. Put the cleaned CSV inside the repository's `data/` folder.
6. Add screenshots to `screenshots/`.

### Important
Potential outliers are reported rather than automatically deleted. An unusual value may be a valid observation, so deletion should be supported by domain evidence.

### Outcome
The project produces a documented, validated cleaned dataset and a set of visual analyses suitable for a beginner Data Science portfolio and GIST Task 1 submission.

# GIST Data Science Internship — Task 3
## Data Analysis & Prediction

### Objective
This project completes GIST Data Science Task 3 by preparing a dataset, performing feature engineering, analyzing important variables, training predictive models, tuning the stronger model, evaluating performance, and documenting the findings.

### Dataset
Student Performance Factors — Kaggle:
https://www.kaggle.com/datasets/lainguyn123/student-performance-factors

### Target
`Exam_Score`

### Workflow
1. Load and inspect data
2. Remove duplicate records
3. Engineer interpretable predictor features
4. Analyze correlations
5. Split data into train/test sets
6. Build preprocessing pipeline
7. Train Random Forest Regressor
8. Train Gradient Boosting Regressor
9. Compare MAE, RMSE and R²
10. Tune the stronger model with randomized cross-validation
11. Evaluate actual vs predicted values
12. Analyze feature importance and prediction errors
13. Export prediction/model-analysis files

### Technologies
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Google Colab

### Files
- `GIST_Task3_Data_Analysis_Prediction.ipynb`
- `README.md`
- `data/` — optional exported data

### Reproducibility
Open the notebook in Google Colab and run all cells from top to bottom. The notebook downloads the public dataset with `kagglehub`.

### Evaluation
The project uses:
- MAE — average absolute prediction error
- RMSE — penalizes larger errors more strongly
- R² — proportion of target variance explained by the model

### Modeling note
`Exam_Score` is excluded from the input features to avoid target leakage. Missing-value handling is performed inside the preprocessing pipeline so that the test set does not influence training-time imputation.

### Interpretation note
Correlation and model feature importance indicate association/predictive usefulness; they do not establish causation.

# GIST Data Science Internship — Task 4

## Advanced + Interactive Data Dashboard

This project completes **GIST Data Science Task 4**, which requires building an interactive dashboard using tools like Plotly, Streamlit, Power BI, or Tableau. The dashboard must connect to a dataset, include filters and KPIs, visualize trends, and generate actionable insights.

## Project Objective

Build an interactive **Sales Performance Dashboard** using Plotly in Python to analyze revenue, profit, and business performance across different dimensions.

## Dataset

**Retail Sales Dataset (Synthetic)**

The dataset contains transaction-level data including:

* `OrderID`
* `Date`
* `Region`
* `Category`
* `Segment`
* `Revenue`
* `Profit`

The dataset is generated programmatically for reproducibility and portfolio demonstration.

## Features Implemented

### KPI Metrics

* Total Revenue
* Total Profit
* Total Orders
* Average Order Value
* Profit Margin

### Filters

* Region filter
* Category filter

### Visualizations

* Monthly Revenue Trend (Line Chart)
* Revenue by Category (Bar Chart)
* Revenue by Region (Pie Chart)
* Profit vs Revenue (Scatter Plot)

### Actionable Insights

* Top-performing category
* Best-performing region
* Profitability analysis
* Sales trend evaluation

## Project Workflow

1. Generate or load dataset
2. Perform feature engineering (extract month from date)
3. Calculate KPIs
4. Apply filters (Region, Category)
5. Aggregate data for analysis
6. Create interactive visualizations using Plotly
7. Generate business insights based on data

## How to Run

1. Open Google Colab
2. Copy the notebook/code into a new notebook
3. Install dependencies:

   ```bash
   pip install plotly pandas
   ```
4. Run all cells from top to bottom
5. Modify filter variables in code to explore different results

## Dashboard KPIs

* **Total Revenue** — sum of all revenue
* **Total Profit** — sum of all profit
* **Total Orders** — number of unique orders
* **Average Order Value (AOV)** — Revenue / Orders
* **Profit Margin (%)** — (Profit / Revenue) × 100

## Actionable Insights Logic

The dashboard dynamically identifies:

* Highest revenue-generating category
* Best-performing region
* Low profit margin warning
* Declining sales trends

These insights help simulate real-world business decision-making.

## Files

* `GIST_Task4_Interactive_Dashboard.ipynb` — complete Colab notebook
* `README.md` — project documentation

## Technologies

* Python
* Pandas
* NumPy
* Plotly
* Google Colab

## GIST Task 4 Requirements Checklist

* Dataset connected 
* KPIs implemented 
* Filters applied 
* Trends visualized 
* Interactive charts 
* Actionable insights 

## Outcome

The project delivers a fully functional interactive dashboard that enables users to explore data, understand key metrics, identify trends, and make data-driven decisions. It demonstrates practical skills in data analysis, visualization, and business storytelling.
