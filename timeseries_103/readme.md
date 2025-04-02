# ⏱️ Time Series 103 – Advanced Time Series Analysis

This module is part of the [Time Series Tutorial](https://github.com/PantosThn/timeseries_tutorial) series and focuses on advanced time series concepts, modeling pipelines, decomposition, forecasting, and evaluation techniques.

> 📚 Recommended: Complete `timeseries_101` and `timeseries_102` before diving in.

## 🔧 Setup

This project uses [Poetry](https://python-poetry.org/) for environment and dependency management. Optionally, you can speed up installs using [uv](https://github.com/astral-sh/uv).

### 1. Install Poetry and optionally uv

```bash
pip install poetry
# Optional: for faster installs
pip install uv
```

### 2. Clone the repository and navigate to this module

```bash
git clone https://github.com/PantosThn/timeseries_tutorial.git
cd timeseries_tutorial/timeseries_103
```

### 3. Run setup (with plugin installation, dependency install, and environment activation)

```bash
# Inside timeseries_103/
poetry self add poetry-plugin-export
poetry self add poetry-plugin-shell

poetry install --sync --with dev -E all

# Optional: Fast install using uv (after adding export plugin)
uv pip install -r <(poetry export --without-hashes --with dev --extras all -f requirements.txt)

# Activate environment (either way works)
poetry shell
# OR
source $(poetry env info --path)/bin/activate
```

---

## ▶️ Usage

Launch JupyterLab or Jupyter Notebook to explore the tutorials:

```bash
jupyter lab
# or
jupyter notebook
```

---

## 📁 Structure

- `notebooks/`: Interactive tutorials in notebook format  
- `scripts/`: Utility functions and modeling helpers  
- `data/`: Sample datasets or download scripts  
- `pyproject.toml`: Dependency and project configuration  

---

## 🧠 Topics Covered

- Time series decomposition  
- Feature engineering  
- Forecasting pipelines  
- Model evaluation  
- Real-world time series examples  

---

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## 📜 License

MIT License
