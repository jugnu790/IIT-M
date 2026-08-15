# IIT-M Data Analysis Assignments

Assignments are organised by day. Each assignment contains its own `code`, `data`, `output`, and `report` folders, with a README describing the submitted work.

A structured collection of Python data-analysis assignments completed as part of the IIT-M coursework. The repository is organized day-wise and contains Jupyter notebooks, assignment documentation, datasets, reports, and generated outputs where applicable.

## 📚 Repository Overview

The project is organized into four working days:

```text
IIT-M/
├── Day 1/
│   └── Assignment 1/
│       ├── README.md
│       └── code/
│           └── numpy_array_slicing.ipynb
│
├── Day 2/
│   └── Assignment 1/
│       ├── README.md
│       └── code/
│           └── python_basics_arrays_dictionaries.ipynb
│
├── Day 3/
│   ├── Assignment 1/
│   ├── Assignment 2/
│   ├── Assignment 3/
│   ├── Assignment 4/
│   ├── Assignment 5/
│   └── Assignment 6/
│
├── Day 4/
│   └── Assignment 1/
│       ├── README.md
│       ├── code/
│       │   └── patient_clinical_data_analysis.ipynb
│       ├── data/
│       └── output/
│
├── .gitignore
├── .python-version
├── pyproject.toml
├── requirements.txt
└── README.md
```

> The exact contents of individual assignment folders may grow as additional notebooks, reports, datasets, and outputs are completed.

## 🎯 Objectives

The assignments focus on practical Python-based data analysis, including:

- Python fundamentals
- NumPy arrays and array slicing
- Lists, dictionaries, and data structures
- Pandas-based data manipulation
- Data cleaning and transformation
- Exploratory Data Analysis (EDA)
- Statistical analysis
- Data visualization
- Working with CSV and Excel data
- Communicating analytical findings through notebooks and reports

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python 3.12+ | Core programming language |
| uv | Python environment and package management |
| JupyterLab | Interactive notebook environment |
| Jupyter Notebook | Assignment execution |
| NumPy | Numerical computing and array operations |
| Pandas | Data manipulation and analysis |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| SciPy | Scientific and statistical computing |
| OpenPyXL | Excel file handling |
| Git | Version control |

The repository is configured for Python 3.12 through `.python-version`, while `pyproject.toml` requires Python 3.12 or newer.

## 🚀 Setup

### 1. Clone the repository

```powershell
git clone <your-repository-url>
cd IIT-M
```

### 2. Create the virtual environment

```powershell
uv venv --python 3.12
```

### 3. Activate the environment

PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

You should see:

```text
(IIT-M) PS D:\IIT-M>
```

### 4. Install dependencies

```powershell
uv pip install -r requirements.txt
```

### 5. Verify the environment

```powershell
uv pip check
```

You should get:

```text
All installed packages are compatible
```

You can also verify the main libraries:

```powershell
python -c "import pandas, numpy, matplotlib, seaborn, scipy; print('Environment OK')"
```

## 📓 Jupyter / VS Code

The project is designed to run through Jupyter notebooks in VS Code or JupyterLab.

Register the environment as a Jupyter kernel:

```powershell
python -m ipykernel install --user --name iitm-data-analysis --display-name "IIT-M Data Analysis"
```

Verify:

```powershell
jupyter kernelspec list
```

The selected kernel should use the project's virtual environment:

```text
D:\IIT-M\.venv\Scripts\python.exe
```

Inside a notebook, the environment can be verified with:

```python
import sys
print(sys.executable)
```

## ▶️ Running an Assignment

From the repository root:

```powershell
.\.venv\Scripts\Activate.ps1
code .
```

Then:

1. Open the required `Day X` folder.
2. Open the required assignment.
3. Open the notebook inside the `code` folder.
4. Select the `IIT-M Data Analysis` kernel.
5. Run the notebook cells.
6. Review the outputs and findings.
7. Save the notebook.

For data-driven assignments, keep datasets in the assignment's `data` directory and use relative paths from the notebook location.

Example:

```python
import pandas as pd

df = pd.read_csv("data/your_dataset.csv")
```

## 🧪 Recommended Notebook Structure

For analytical assignments, a consistent notebook structure makes the work easier to understand and review:

```text
1. Objective
2. Import Libraries
3. Load Dataset
4. Dataset Understanding
5. Data Cleaning
6. Data Transformation
7. Exploratory Data Analysis
8. Analysis
9. Visualizations
10. Key Findings
11. Conclusion
```

Use **Markdown cells** for explanations and interpretation, and **Code cells** for implementation.

## 📦 Dependencies

The current project dependency list is maintained in:

```text
requirements.txt
```

Current core dependencies:

```text
pandas
numpy
matplotlib
seaborn
jupyterlab
openpyxl
scipy
```

Install them with:

```powershell
uv pip install -r requirements.txt
```

## 🔐 Data & Privacy

Do not commit sensitive, confidential, or personally identifiable information to a public repository.

In particular, datasets containing real patient or other private information should not be publicly uploaded unless they are explicitly safe and authorized for public distribution.

The repository ignores common local/environment files such as:

```text
.venv/
__pycache__/
.ipynb_checkpoints/
*.pyc
```

## 🌿 Git Workflow

A simple workflow for each completed assignment:

```powershell
git status
git add "Day X/Assignment Y"
git commit -m "Complete Day X Assignment Y"
git push
```

Before pushing, always check:

```powershell
git status
```

This prevents accidentally committing virtual environments, temporary files, notebook checkpoints, or unrelated changes.

## 📈 Progress

| Day | Status |
|---|---|
| Day 1 | 🟢 In progress / completed assignments as committed |
| Day 2 | 🟢 In progress / completed assignments as committed |
| Day 3 | 🟢 In progress / completed assignments as committed |
| Day 4 | 🟢 In progress / completed assignments as committed |

Update this table as the coursework progresses rather than marking assignments complete before they are actually finished.

## 📌 Notes

- Keep the existing project structure consistent.
- Use the same Python environment for all assignments.
- Avoid installing packages globally when they belong to this project.
- Prefer `uv` for environment and dependency management.
- Keep notebooks reproducible by using relative file paths.
- Run all relevant notebook cells before committing a completed assignment.
- Do not commit `.venv` or other generated environment files.

## 👤 Author

**Deepesh Upadhyay**

This repository is maintained as a personal coursework and learning portfolio for practical data-analysis work.
