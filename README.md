# Demand-Forecasting-in-E-commerce-with-Time-Series-Data
A machine-learning project for forecasting weekly retail product demand using historical sales, pricing, store, SKU, and promotional features.

## Overview

Accurate demand forecasting helps retailers make better decisions about inventory management, replenishment, pricing, and promotions.

This project analyzes historical retail sales data and applies multiple forecasting and machine-learning techniques to predict the number of units sold for products across different stores and weeks.

The dataset contains:

- 150,150 sales records
- 130 weeks of historical data
- Multiple stores and products
- Product pricing information
- Promotional indicators
- Weekly unit sales as the target variable

## Objective

The primary objective is to predict:

```text
units_sold
```

The prediction is based on features such as:

- Week
- Store ID
- SKU ID
- Total price
- Base price
- Featured SKU indicator
- Display promotion indicator
- Historical sales patterns

## Dataset Features

| Feature | Description |
|---|---|
| `record_ID` | Unique identifier for each sales record |
| `week` | Week in which the sale occurred |
| `store_id` | Unique identifier of the store |
| `sku_id` | Unique identifier of the product |
| `total_price` | Selling price of the product |
| `base_price` | Regular/base price of the product |
| `is_featured_sku` | Indicates whether the product was featured |
| `is_display_sku` | Indicates whether the product was placed on display |
| `units_sold` | Number of units sold; prediction target |

## Project Workflow

The notebook follows these main steps:

1. Load the retail sales dataset.
2. Inspect the structure and quality of the data.
3. Convert the `week` column into a datetime format.
4. Aggregate and analyze weekly sales.
5. Explore demand trends and sales patterns.
6. Prepare features for model training.
7. Train multiple forecasting and regression models.
8. Generate predictions for product demand.
9. Compare model performance.
10. Identify a suitable model for demand forecasting.

## Models

The project evaluates multiple models for predicting retail demand. The models may include statistical forecasting methods and machine-learning algorithms such as:

- Time-series forecasting models
- Linear regression models
- Tree-based regression models
- Ensemble models
- Other machine-learning approaches implemented in the notebook

Model performance can be compared using regression metrics such as:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- R² score

## Tech Stack

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Time-series forecasting libraries, where applicable

## Installation

Clone the repository:

```bash
git clone [https://github.com/](https://github.com/)<your-username>/<your-repository>.git
cd <your-repository>
```

Create and activate a virtual environment:

```bash
python -m venv venv
```

On macOS or Linux:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook:

```text
Use_Case_3_Demand_Forecasting_All_Models.ipynb
```

Run the notebook cells in order to:

- Load and explore the data
- Perform preprocessing
- Train the forecasting models
- Generate predictions
- Evaluate and compare model performance

## Example Prediction Task

The project uses historical information such as pricing, promotions, store identity, product identity, and previous sales trends to estimate future demand:

```text
Input:
- Store
- Product
- Selling price
- Base price
- Promotion indicators
- Historical demand

Output:
- Expected units sold
```

## Business Applications

The forecasting solution can support:

- Inventory replenishment
- Stock-level optimization
- Store-level planning
- Product-level demand estimation
- Promotion analysis
- Pricing decisions
- Reduction of overstock and stockouts

## Results

The notebook compares the performance of the implemented models and identifies the models that provide the most accurate demand predictions.

For the final version of this README, add the best-performing model and its evaluation metrics here:

```text
Best model: <model-name>
RMSE: <value>
MAE: <value>
MAPE: <value>
R² score: <value>
```

## Project Structure

```text
.
├── Use_Case_3_Demand_Forecasting_All_Models.ipynb
├── data/
│   └── retail_demand.csv
├── requirements.txt
└── README.md
```

## Future Improvements

Potential improvements include:

- Adding lag-based demand features
- Including rolling averages and rolling standard deviations
- Creating holiday and seasonal indicators
- Incorporating additional store-level information
- Performing hyperparameter tuning
- Using cross-validation designed for time-series data
- Deploying the best model as an API
- Creating an interactive demand-forecasting dashboard
- Adding automated model retraining

## Limitations

- Forecast accuracy depends on the quality and completeness of the historical data.
- External factors such as holidays, weather, competitors, and supply disruptions may not be included.
- Random train-test splits should be avoided for time-series forecasting because they can cause data leakage.
- Model performance may vary between stores and products.

## Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch:

```bash
git checkout -b feature/new-improvement
```

3. Commit your changes:

```bash
git commit -m "Add new forecasting improvement"
```

4. Push the branch:

```bash
git push origin feature/new-improvement
```

5. Open a pull request.

## License

This project is available under the MIT License. Add a `LICENSE` file to the repository if you would like to distribute the project under this license.

## Author

**Sanjeevteja Ponugumati**

Data Scientist  
Bengaluru, Karnataka, India


