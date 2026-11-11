# 02807 Computational Tools Project

Project scaffold for preparing Steam interaction data, exploring and filtering it,
building a MinHash/LSH model, and performing graph analysis.

## Structure

- `data/raw/`: source datasets
- `data/interim/`: intermediate data produced during preprocessing
- `data/processed/`: cleaned datasets used by later analyses
- `notebooks/`: numbered analysis workflow
- `src/`: reusable Python modules
- `figures/`: generated plots and diagrams

## Setup

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

## Getting the data

The datasets are available from the
[Steam Video Game and Bundle Data page](https://cseweb.ucsd.edu/~jmcauley/datasets.html#steam_data).
Download these two files:

- [Version 1: User and Item Data](https://mcauleylab.ucsd.edu/public_datasets/data/steam/australian_users_items.json.gz) (71 MB)
- [Version 2: Item Metadata](https://cseweb.ucsd.edu/~wckang/steam_games.json.gz) (2.7 MB)

Save both files in `data/raw/`, retaining their original filenames:

```text
data/raw/australian_users_items.json.gz
data/raw/steam_games.json.gz
```

Files under `data/` are excluded from Git. After downloading the raw datasets,
run the notebooks in numerical order.
