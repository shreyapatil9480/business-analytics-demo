# Business Analytics Project

This repository contains a synthetic business dataset and an accompanying analysis notebook designed to showcase the skills of a business analyst, program manager, or data analyst. The goal is to provide a self‑contained example that demonstrates data manipulation, exploratory analysis and predictive modelling.

## Repository structure

| File | Description |
| --- | --- |
| `synthetic_business_data.csv` | The synthetic dataset containing customer and transaction information. |
| `analysis_notebook.ipynb` | A Jupyter notebook that performs EDA, builds regression and classification models, and summarises findings. |
| `requirements.txt` | A list of Python packages required to run the notebook. |
| `README.md` | This file; provides an overview of the project and instructions. |

## Dataset description

The dataset contains 1,000 rows with the following columns:

| Column | Type | Description |
| --- | --- | --- |
| `CustomerID` | integer | Unique identifier for each customer. |
| `Gender` | categorical | Customer gender (Male/Female). |
| `Age` | integer | Customer age in years. |
| `Region` | categorical | Geographic region (North, South, East, West). |
| `ProductCategory` | categorical | Product category (Electronics, Clothing, Home, Beauty, Sports). |
| `Date` | date | Date of transaction within the past three years. |
| `UnitsPurchased` | integer | Number of units purchased in the transaction. |
| `UnitPrice` | float | Price per unit (USD). |
| `MarketingSpend` | float | Marketing spend associated with the transaction (USD). |
| `Revenue` | float | Total revenue generated (`UnitsPurchased` × `UnitPrice`). |
| `HighPurchase` | integer | Indicator of high purchase activity (1 if units > 5 or marketing spend > $100, else 0). |

## Getting started

To explore this project, clone or download the repository and install the required dependencies using pip:

```bash
pip install -r requirements.txt
```

Then open the Jupyter notebook to run the analysis:

```bash
jupyter notebook analysis_notebook.ipynb
```

## Potential extensions

This project is intentionally simple and ready to use, but there are many ways you could extend it:

- Increase the dataset size or complexity by adding features such as loyalty status, time of day, or promotional codes.
- Perform customer segmentation using clustering algorithms.
- Build time series forecasts on aggregated revenue data.
- Explore classification algorithms beyond logistic regression (e.g. random forests, gradient boosting).
- Deploy predictive models as a microservice.

Feel free to adapt this repository to suit your interests and to demonstrate your analytical capabilities.

## Usage example

After cloning the repository and installing the dependencies, you can run the notebook to explore the dataset and build models. Below is a quick summary of the steps:

1. Load the synthetic data using pandas.
2. Use seaborn and matplotlib to visualize key relationships, such as revenue by product category or correlation between marketing spend and units purchased.
3. Fit a regression model to predict revenue using features like units purchased and marketing spend.
4. Fit a classification model to identify high purchase activity.

Refer to the `analysis_notebook.ipynb` for the complete analysis and code.
