# RFM and CLV Analysis for Online Sales Data

## Overview

This project performs **Recency, Frequency, and Monetary (RFM) analysis** and **Customer Lifetime Value (CLV) calculation** on an online sales dataset. The script loads transaction data, processes it to derive key customer insights, and visualizes customer segments.

## Features

- Loads and preprocesses an online sales dataset
- Computes **RFM (Recency, Frequency, Monetary) analysis**
- Assigns **RFM scores** and segments customers
- Calculates **Customer Lifetime Value (CLV)** using discounted revenue over a given time horizon
- Provides **data visualization** for better insights
- Exports results to CSV

## Dataset

The script expects a CSV file (`Online_Sales.csv`) with the following columns:

- `Transaction_ID`: Unique transaction identifier
- `CustomerID`: Unique customer identifier
- `Transaction_Date`: Date of transaction
- `Quantity`: Number of items purchased
- `Avg_Price`: Average price per item

## Installation

To run this project, ensure you have Python installed along with the following dependencies:

```bash
pip install pandas numpy matplotlib seaborn
```

## Usage

1. Place the dataset (`Online_Sales.csv`) in the same directory as the script.
2. Update the `file_path` variable in the script if needed.
3. Run the script:

```bash
python rfm_clv_analysis.py
```

4. The output includes:
   - **RFM analysis results**
   - **CLV calculations per customer**
   - **Data visualizations**
   - **Exported CSV file (****`rfm_clv_analysis.csv`****)**

## Key Calculations

### 1. RFM Analysis

- **Recency**: Days since the last transaction
- **Frequency**: Number of unique transactions
- **Monetary**: Total revenue per customer
- **RFM Score**: Combination of individual scores assigned based on quartiles

### 2. CLV Calculation

- Uses a **discounted revenue model** over a defined time horizon (default: 12 months)
- Assumes a **10% discount rate** to calculate future customer value

## Visualizations

The script generates scatter plots for customer insights:

- **Recency vs. Frequency**
- **Frequency vs. Monetary**
- **Recency vs. Monetary**

## Output

The processed data with RFM and CLV scores is saved as `rfm_clv_analysis.csv`.

## License

This project is open-source under the [MIT License](LICENSE).

## Author

Vishnu Prasad V (vishnuprasad\@sjmsom.in)

