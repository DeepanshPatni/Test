# Energy Consumption Forecasting for Smart Grid Optimization

This project aims to analyze, predict, and optimize energy consumption patterns in smart homes using machine learning techniques. By leveraging high-frequency data from smart meters, the system can provide actionable insights for energy efficiency and grid optimization.

## **Project Overview**
As energy consumption patterns grow more complex due to renewable resources, this project addresses the need for efficient analysis and optimization. The workflow includes forecasting, clustering, and classification tasks to improve energy management and support smart grid optimization.

### **Key Features**
1. **Data Preprocessing**:
   - Imputation of missing values using mean/mode for numerical features.
   - Aggregation of minute-level data to daily totals for trend analysis.
   - Feature standardization and correlation-based feature removal.

2. **Forecasting**:
   - **ARIMA**: Predicts energy consumption using historical data trends.
   - **SARIMAX**: Enhances ARIMA by incorporating external factors (e.g., temperature, humidity).
   - **Metrics**:
     - ARIMA: RMSE = 273.41 kW, MAPE = 17.2%.
     - SARIMAX: RMSE = 294.79 kW, MAPE = 18.21%.

3. **Clustering**:
   - **K-Means** clustering identifies consumption behavior:
     - **High Consumption**: Peak energy users.
     - **Medium Consumption**: Average users.
     - **Low Consumption**: Energy-efficient users.

4. **Classification**:
   - **Random Forest** classifier labels energy usage as "efficient" or "inefficient" for actionable insights.
   - Accuracy: 95.33%.

## **Workflow**
1. Data collection from smart meters and weather sources.
2. Data preprocessing and exploratory data analysis.
3. Training models:
   - Time-series forecasting (ARIMA, SARIMAX).
   - Clustering (K-Means).
   - Classification (Random Forest).
4. Model evaluation using RMSE, MAPE, and Accuracy metrics.

## **Results**
- **Forecasting**: SARIMAX provides interpretability with external weather features, while ARIMA offers slightly better error metrics.
- **Clustering**: Reveals distinct energy usage patterns for tailored solutions.
- **Classification**: Accurately identifies inefficient energy usage for optimization.

## **Technologies Used**
- Python (NumPy, Pandas, scikit-learn, statsmodels)
- Graphviz (for visualizations)
- Matplotlib and Seaborn (for data visualization)

## **How to Run**
1. Clone the repository.
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
