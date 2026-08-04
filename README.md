# Tesla and GameStop Stock and Revenue Analysis

This project extracts and visualizes historical stock-price and quarterly-revenue data for Tesla and GameStop.

It was completed as part of the IBM Data Science Professional Certificate and subsequently cleaned, debugged, and documented for my portfolio.

## Project objectives

The project demonstrates how Python can combine financial data from multiple sources. Its objectives are to:

- Extract historical stock data using `yfinance`
- Scrape quarterly revenue tables using Beautiful Soup
- Clean date and currency values using pandas
- Compare share-price history with reported revenue
- Create interactive visualizations using Plotly
- Present the analysis in a reproducible Jupyter notebook

## Technologies used

- Python
- Jupyter Notebook
- pandas
- yfinance
- Requests
- Beautiful Soup
- Plotly
- Visual Studio Code
- Git and GitHub

## Project structure

```text
tesla-gamestop-stock-analysis/
├── Final Assignment.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Data sources

### Historical stock data

Historical Tesla and GameStop share-price data is retrieved from Yahoo Finance through the `yfinance` Python package.

## Key findings

The visualizations show that share-price movements do not always follow reported company revenue directly.

Tesla’s chart shows substantial growth in both market value and revenue over the period, although the two measures do not move in identical patterns.

GameStop’s chart demonstrates a particularly large difference between market activity and the company’s reported revenue trend. This highlights how investor behaviour, expectations, and market events can affect share prices independently of current revenue.

These charts demonstrate correlation and timing patterns, but they do not establish that revenue changes directly caused stock-price changes.


## Acknowledgements

The original assignment structure and source datasets were provided by IBM Skills Network as part of the IBM Data Science Professional Certificate.

The completed analysis, debugging, data-cleaning improvements, environment setup, project organization, and portfolio documentation are presented here as my coursework.
