# AGENTS.md

## Cursor Cloud specific instructions

This is an educational data science project with Jupyter notebooks. There is no web application, backend, or database.

### Key files
- `Unstructured_Data_gain.ipynb` / `Unstructured Data.ipynb` — Jupyter notebooks covering pandas, JSON normalization, TF-IDF, and LBP image features
- `app.py` — empty stub (no functionality)
- `git_gianl.py` — simple test script (`python3 git_gianl.py`)
- `online_retail_II.xlsx` — ~44 MB dataset used by the notebooks

### Running
- Start Jupyter Lab: `jupyter lab --no-browser --ip=0.0.0.0 --port=8888 --ServerApp.token='' --ServerApp.password=''`
- Run a script: `python3 git_gianl.py`
- The `~/.local/bin` directory must be on PATH for `jupyter` and other pip-installed scripts.

### Python packages required
`pandas`, `numpy`, `openpyxl`, `pyarrow`, `scikit-learn`, `scikit-image`, `Pillow`, `datasets`, `jupyterlab`

### Gotchas
- No `requirements.txt` exists in the repo; packages are installed manually via pip.
- The Excel dataset has mixed-type columns (`Invoice`, `StockCode`); convert object columns to `str` before writing to Parquet.
- Some notebook exercises download external data (companies.json from GitHub, HuggingFace dataset); these require internet access.
- There are no automated tests or lint configurations in this project.
