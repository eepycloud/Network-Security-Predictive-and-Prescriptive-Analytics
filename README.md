

## Project Objectives
- **Predictive Analytics:** Develop models to forecast key network metrics such as Time-to-Live (TTL), Hop Count, and Rate of Energy Consumption.
- **Prescriptive Analytics:** Determine optimal strategies for minimizing risk scores across network nodes.
- **Implementation:** Use Python to implement predictive and prescriptive models.
- **Presentation:** Deliver a comprehensive presentation detailing the methodology, findings, and actionable recommendations.

## Key Components
- **Predictive Modeling:**
  - Feature selection techniques: Select From Model, SelectKBest, Forward/Backward Sequential Feature Selector, Recursive Feature Elimination.
  - Regression models: Linear Regression, K-Nearest Neighbor Regression (KNNR), Support Vector Regression (SVR), Decision Tree Regression (DTR), Random Forest Regressor.
  - Evaluation metrics: RMSE, MAE, MSE, R-squared.
  
- **Prescriptive Analytics:**
  - Optimization of risk score using a weighted formula considering TTL, Hop Count, and Rate of Energy Consumption.
  - Constraint-based optimization to minimize risk while ensuring network security.

## Repository Contents
- **Notebooks:**
  - `predictive_analytics.ipynb`: Contains the code and analysis for predictive modeling.
  - `prescriptive_analytics.ipynb`: Contains the code and analysis for prescriptive modeling.
  
- **Presentation:**
  - `presentation.pptx`: A PowerPoint presentation summarizing the methodology, results, and recommendations.

## How to Run
1. Clone the repository.
2. Open the notebooks in Google Colab or Jupyter.
3. Run the cells to reproduce the analysis.

## Requirements
- Python 3.x
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
  
## Data
- **The data set that was used for part 1 will be found here in this link:** [Download Here](https://drive.google.com/file/d/1uk8_KFIKkYKsR2ZoH4nbn1heX2OqDQUf/view?usp=sharing)
- **The data set that was used for part 2 and part 3 (GA_PSO) will be found here in this link** [Download Here](https://drive.google.com/file/d/1PRI2NuJPBIk_P79ROy6C15OytN7F4PjD/view?usp=sharing)
- **Metadata:** The `metadata.txt` file explains the columns and features used in the analysis.
  
## References
All code and analysis are based on the tasks outlined in the assignments from the Data Analytics course at HTU.
 
