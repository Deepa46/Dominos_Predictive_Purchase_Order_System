## Dominos_Predictive_Purchase_Order_System

### Overview
This project aims to forecast the ingredients required for pizzas based on historical sales data using the Arima model. The system enhances inventory management and minimizes food waste by predicting ingredient needs for the upcoming week.

## Key Components

### 1. Data Exploration and Cleaning
- Conduct an initial analysis of the datasets to understand their structure and quality.
- Handle missing values in the ingredient quantities and detect any outliers for reliable model training.

### 2. Feature Engineering
- Deriving features from existing columns to provide additional context for the predictions.
- Generating time-based features from the `order_date`, such as day of the week, day of the year, and month, to improve predictive capabilities.


### 3. Model Training
- Train the Arima model on historical sales data to predict future ingredient requirements.
- Fine-tune model parameters to enhance accuracy and reliability.

### 4. Model Evaluation
- Evaluate model performance using Mean Absolute Percentage Error (MAPE) to ensure the predictions meet business needs.

## Datasets
1. **Pizza Ingredients** (`Pizza_ingredients.csv`):
   - Contains ingredient requirements for each pizza type.
   - Key columns: `pizza_name_id`, `pizza_name`, `pizza_ingredients`, `Items_Qty_In_Grams`

2. **Pizza Sales** (`Pizza_Sale.csv`):
   - Includes historical sales data for pizzas.
   - Key columns: `pizza_id`, `order_id`, `pizza_name_id`, `quantity`, `order_date`, `order_time`, `unit_price`, `total_price`, `pizza_size`, `pizza_category`, `pizza_ingredients`, `pizza_name`
