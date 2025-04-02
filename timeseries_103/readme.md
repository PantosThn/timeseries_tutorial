# Time Series Tutorial

This repository demonstrates various time series forecasting techniques and tools.

## Prerequisites

- **Python 3.10+**  
  Make sure you have at least Python 3.10 installed on your machine.

- **[Poetry](https://python-poetry.org/docs/#installation)**  
  For managing dependencies and creating the virtual environment.

- **Optional**: [VS Code](https://code.visualstudio.com/) (with the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python))  
  Recommended if you plan to develop and run notebooks in VS Code.

---

## Installation & Setup

1. **Clone the Repository**

    ```bash
    git clone https://github.com/PantosThn/timeseries_tutorial.git
    cd timeseries_tutorial/timeseries_103
    ```

2. **Select Python Interpreter and Install Dependencies**  
   Ensure you have Python 3.10+ installed, then run:

    ```bash
    poetry env use python3.10
    poetry install
    ```

   - `poetry env use python3.10` instructs Poetry to create/use a virtual environment with Python 3.10.  
   - `poetry install` installs all required dependencies listed in `pyproject.toml`.

3. **Activate the Virtual Environment**

    ```bash
    poetry shell
    ```

   Your terminal prompt may change (e.g., to `Py timeseries-103-py3.10`), indicating that you’re now inside the `.venv`.

4. **(Optional) Register a Jupyter Kernel**

    If you plan to use Jupyter notebooks, install a kernel spec for this environment:

    ```bash
    python -m ipykernel install --user --name=timeseries-103 --display-name "Python (timeseries-103)"
    ```

    This creates a Jupyter kernel named `timeseries-103` so you can select it in Jupyter or VS Code.

---

## Running Jupyter Notebooks

1. **Launch Jupyter**  
   Inside your Poetry shell, run:

    ```bash
    jupyter notebook
    ```
   or
    ```bash
    jupyter lab
    ```

2. **Select the Kernel**  
   In the browser tab, open a notebook (`.ipynb`). Then choose “Python (timeseries-103)” from the kernel selection dropdown if you used the `ipykernel install` command above.

---

## Using VS Code

If you want to work in VS Code:

1. **Open the Correct Folder**  
   Make sure you open the `timeseries_103` folder in VS Code (either directly or as part of the parent workspace).

2. **Select the Poetry Environment**  
   - Press <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> (Windows/Linux) or <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> (macOS).  
   - Type “Python: Select Interpreter” and pick the interpreter that points to:
     ```
     .../timeseries_103/.venv/bin/python
     ```

3. **Run or Open Notebooks**  
   - Create or open a `.ipynb` file.
   - In the top-right corner of the notebook, choose the kernel named `Python (timeseries-103)`.
   - Now your notebook cells will run in the Poetry-managed virtual environment.

---

## Contributing

1. [Fork the repo](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo) (if you’re on GitHub).
2. Create a new branch for your changes.
3. Make your improvements or updates.
4. Submit a pull request.

---

## License

[MIT License](LICENSE) - or use whichever license suits your project.
