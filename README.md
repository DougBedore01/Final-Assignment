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

- `Final Assignment.ipynb` contains the analysis, explanations, tables, and visualizations.
- `README.md` explains the project and how to run it.
- `requirements.txt` lists the required Python packages.
- `.gitignore` prevents temporary and machine-specific files from being uploaded.

## How to run the project

These instructions allow another user to recreate the Python environment and run the analysis on their own computer.

### 1. Clone the repository

```bash
git clone REPLACE-WITH-YOUR-REPOSITORY-URL
```

This command downloads the GitHub repository and its files to the user’s computer.

Enter the downloaded project folder:

```bash
cd tesla-gamestop-stock-analysis
```

This changes the terminal’s working location so that subsequent commands run inside the project.

### 2. Create a virtual environment

On Windows:

```powershell
python -m venv .venv
```

This uses Python’s built-in `venv` module to create an isolated environment named `.venv`. Isolation prevents this project’s packages from interfering with packages used by other projects.

### 3. Activate the virtual environment

```powershell
.venv\Scripts\Activate.ps1
```

This makes the terminal use the Python installation inside `.venv`. After activation, the terminal prompt should begin with `(.venv)`.

### 4. Install the dependencies

```powershell
python -m pip install -r requirements.txt
```

This asks the activated Python environment to install every package listed in `requirements.txt`.

### 5. Open and run the notebook

Open `Final Assignment.ipynb` in VS Code or Jupyter Notebook.

In VS Code:

1. Select the `.venv` Python environment as the notebook kernel.
2. Click **Run All**.
3. Allow the notebook to download the stock and revenue data.
4. Review the tables and interactive charts produced by the cells.

Running the cells from top to bottom ensures that imports, variables, downloaded data, cleaning steps, and plotting functions are created in the correct order.

## Data sources

### Historical stock data

Historical Tesla and GameStop share-price data is retrieved from Yahoo Finance through the `yfinance` Python package.

The relevant ticker symbols are:

- Tesla: `TSLA`
- GameStop: `GME`

### Quarterly revenue data

Quarterly revenue data is extracted from HTML pages supplied through the IBM Skills Network course materials.

The notebook uses `requests` to download the HTML and Beautiful Soup to locate and extract the relevant tables.

## Data preparation

The revenue information initially contains formatted text values such as:

```text
$1,021
```

The notebook removes dollar signs and commas before converting the values into numbers. Dates are also converted into pandas datetime values.

These cleaning steps are necessary because charts and numerical operations require consistent numeric and date data types rather than formatted text
```
