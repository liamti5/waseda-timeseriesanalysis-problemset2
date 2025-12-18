# Time Series Analysis - Problem Set 2

This repository contains solutions to Problem Set 2 for Time Series Analysis at Waseda University.

## Project Structure

```
tsa_ps2/
├── data/
│   ├── NASDAQCOM.csv          # NASDAQ composite index data
│   ├── SP500.csv              # S&P 500 index data
│   ├── UNRATE.csv             # Unemployment rate data
│   └── exercise2/
│       ├── FEDFUNDS.csv       # Federal funds rate
│       ├── GDPC1.csv          # Real GDP
│       ├── GDPDEF.csv         # GDP deflator
│       ├── M2SL.csv           # M2 money supply
│       └── PPIACO.csv         # Producer price index
├── notebooks/
│   └── PS2_liam-tessendorf.ipynb  # Main analysis notebook
├── pyproject.toml             # Project dependencies
├── uv.lock                    # Locked dependency versions
└── README.md                  # This file
```

## Prerequisites

- **Python 3.13+** (specified in `pyproject.toml`)
- **[uv](https://docs.astral.sh/uv/)** - Fast Python package installer and resolver

### Installing uv

If you don't have `uv` installed:

**macOS/Linux:**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

**Homebrew:**
```bash
brew install uv
```

**Windows:**
```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

**With pip:**
```bash
pip install uv
```
if none of these options work, check the [installation guide](https://docs.astral.sh/uv/getting-started/installation/#standalone-installer).

## Quick Start

### 1. Clone the Repository

```bash
git clone git@github.com:liamti5/waseda-timeseriesanalysis-problemset2.git
cd waseda-timeseriesanalysis-problemset2
```

### 2. Sync Dependencies

The `uv.lock` file ensures reproducible installations. Run:

```bash
uv sync
```

This will:
- Create a virtual environment (if not present)
- Install all dependencies with exact versions from `uv.lock`
- Set up the project in development mode


### 3. Launch Jupyter Notebook

```bash
uv run jupyter notebook notebooks/PS2_liam-tessendorf.ipynb
```

### 4. View Only HTML file
There is also a HTML file provided, for easy view only of the problem set. 

