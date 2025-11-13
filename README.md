# Replication Data for "Monetary Policy Under High Uncertainty"

## Description

This repository contains the replication dataset for the paper titled:

**"Monetary Policy Under High Uncertainty: Lessons from the 2020-2025 U.S. Experience"**

This file provides a detailed explanation of the data sources, variable definitions, and usage instructions.

---

## Data Sources

All raw data used in this research are publicly available from the following primary sources:

1.  **Economic Policy Uncertainty (EPU) Index**
    *   **Source**: [policyuncertainty.com](https://www.policyuncertainty.com)
    *   **Description**: A news-based index measuring economic policy uncertainty in the United States.

2.  **Michigan Survey of Consumer Expectations (MICH)**
    *   **Source**: Federal Reserve Economic Data (FRED)
    *   **Series ID**: `MICH`
    *   **Link**: [https://fred.stlouisfed.org/series/MICH](https://fred.stlouisfed.org/series/MICH)

3.  **Federal Funds Rate (FEDFUNDS)**
    *   **Source**: Federal Reserve Economic Data (FRED)
    *   **Series ID**: `FEDFUNDS`
    *   **Link**: [https://fred.stlouisfed.org/series/FEDFUNDS](https://fred.stlouisfed.org/series/FEDFUNDS)

4.  **Consumer Price Index (CPI)**
    *   **Source**: U.S. Bureau of Labor Statistics (BLS)
    *   **Available via**: FRED, Series `CPIAUCSL`
    *   **Link**: [https://fred.stlouisfed.org/series/CPIAUCSL](https://fred.stlouisfed.org/series/CPIAUCSL)

5.  **Unemployment Rate (UNRATE)**
    *   **Source**: U.S. Bureau of Labor Statistics (BLS)
    *   **Series ID**: `UNRATE`
    *   **Link**: [https://fred.stlouisfed.org/series/UNRATE](https://fred.stlouisfed.org/series/UNRATE)

---

## Files in This Repository

*   `data.csv`: The final, processed dataset used for the analysis in the paper. It contains 174 quarterly observations from 1982-Q1 to 2025-Q2.

---

## Variable Descriptions

| Column Name    | Description                                                                 |
| :------------- | :-------------------------------------------------------------------------- |
| `date`         | Date of the observation (Quarterly)                                         |
| `FEDFUNDS`     | Federal Funds Effective Rate                                                |
| `CPIAUCSL`     | Consumer Price Index for All Urban Consumers                                |
| `UNRATE`       | Civilian Unemployment Rate                                                  |
| `GDPC1`        | Real Gross Domestic Product                                                 |
| `GDPPOT`       | Real Potential Gross Domestic Product                                       |
| `MICH`         | University of Michigan: Consumer Sentiment                                  |
| `EXPINF5YR`    | 5-Year, 5-Year Forward Inflation Expectation Rate                           |
| `VIXCLS`       | CBOE Volatility Index                                                       |
| `GS10`         | 10-Year Treasury Constant Maturity Rate                                     |
| `T10Y3M`       | 10-Year Minus 3-Month Treasury Constant Maturity Spread                     |
| `M2SL`         | M2 Money Stock                                                              |
| `DCOILWTICO`   | Crude Oil Prices: West Texas Intermediate (WTI)                             |
| `DTWEXBGS`     | Trade Weighted U.S. Dollar Index: Broad, Goods                              |
| `EPU_US`       | Economic Policy Uncertainty Index for the United States                     |
| `Inflation`    | Calculated inflation variable used in the model                             |
| `Output_Gap`   | Calculated output gap variable (derived from `GDPC1` and `GDPPOT`)          |

---

## Usage

To load the dataset in your preferred statistical software:

**R:**
```r
# Load the dataset in R
data <- read.csv("data.csv")
head(data)
```

**Python (with pandas):**
```python
# Load the dataset in Python
import pandas as pd
data = pd.read_csv("data.csv")
print(data.head())
```

---

## Citation

If you use this dataset in your research, please cite the original paper:

> [Author Name(s)]. (2025). "Monetary Policy Under High Uncertainty: Lessons from the 2020-2025 U.S. Experience." *[Journal Name]*, Vol(Issue), pp. xx-xx.

---

## License

This dataset is made available under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**. You are free to share and adapt the material for any purpose, provided you give appropriate credit.

For more details, see [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/).

---

**Repository**: [https://github.com/wansuishan/my-research-data](https://github.com/wansuishan/my-research-data)
