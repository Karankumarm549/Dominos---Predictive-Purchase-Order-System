# DOMINOS-PREDICTIVE PURCHASE ORDER SYSTEM
## DOMAIN:
- Food Service Industry
## INTRODUCTION:
- In this project, the task is to optimize the ingredient ordering process for Dominos by leveraging historical sales data and ingredient information. The goal is to accurately forecast future pizza sales and use these predictions to create an efficient purchase order system. By implementing this solution, Dominos can ensure sufficient stock of ingredients to meet customer demand, minimize waste due to overstocking, and prevent stockouts that disrupt operations. This project integrates predictive modeling with operational planning to enhance inventory management and streamline the purchasing process
## SKILLS TAKEAWAY FROM THIS PROJECT:
- **Data Cleaning and Preprocessing**: Handling missing values, feature engineering, and data transformation.
- **Exploratory Data Analysis (EDA):** Visualizing and understanding sales trends, category distributions, and correlations.
- **Predictive Modeling:** Developing and training machine learning models to forecast sales.
- **Ingredient Analysis:** Calculating ingredient requirements based on sales forecasts and existing recipes.
- **Purchase Order Automation:** Generating purchase orders based on predicted demand.
- **Data Visualization:** Creating detailed and interactive visuals using Matplotlib, Seaborn, and Plotly.
- **Decision-Making Insights:** Leveraging analytical results for inventory optimization and supply chain efficiency.
- **Python Programming:** Applying advanced Python techniques for data analysis, visualization, and modeling.
- **Jupyter Notebook:** Documenting and performing all tasks efficiently within Jupyter Notebook.

## EDA-REPORT:
**Exploratory Data Analysis (EDA)** discovers patterns, relationships, and anomalies in the data.
- **Top-Selling Pizzas**
     - This visualization highlights the top 10 most popular pizzas based on total sales.
     - It helps identify which pizzas are in highest demand among customers.
     - The y-axis represents different pizza names, while the x-axis shows the quantity sold.
     - 
## MODEL COMPARISON: MAPE SCORES
- The table below provides an overview of the performance of various forecasting models, summarized through their Mean Absolute Percentage Error (MAPE) scores. The comparison highlights the ranking and effectiveness of each model in predicting sales.


   | **Model**   | **MAPE** | **Rank** | **Best/Worst** |
   |-------------|----------|----------|----------------|
   | ARIMA       | 0.1976   | 1        |     Best       |
   | Prophet     | 0.2163   | 2        |                |
   | SARIMA      | 0.2327   | 3        |                |
   | LSTM        | 0.2345   | 4        |     Worst      |

## ARIMA MODEL FORECASTING:
This section outlines the process of utilizing the best-performing ARIMA model to forecast future sales effectively:

- **Model Loading:** The ARIMA model, previously trained and saved as best_arima_model.pkl, is loaded to generate accurate sales predictions.
- **Sales Forecasting:** Using the loaded model, sales are forecasted for the next 7 days (n_forecast = 7).

## RESULT:

- The ARIMA model was selected as the best-performing model for forecasting pizza sales, achieving a Mean Absolute Percentage Error (MAPE) of 0.1976. This low error rate demonstrates the model's accuracy and reliability in predicting sales trends. The model's hyperparameters were optimized using AutoARIMA, which automatically identified the best-fit values for p (AR order), d (differencing order), and q (MA order) to ensure optimal performance and stationarity of the time series data.

- By leveraging this fine-tuned ARIMA model, the project successfully forecasted future sales with high precision, enabling the creation of efficient purchase orders and accurate ingredient planning. This approach minimizes waste, prevents stockouts, and streamlines the inventory management process.



