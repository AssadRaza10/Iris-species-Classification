# Iris Data Analysis

This repository contains a Jupyter Notebook performing exploratory data analysis (EDA) and basic modeling on a synthetic Iris dataset.

**Contents**
- Notebook: [iris data analysis.ipynb](iris data analysis.ipynb)
- Dataset: [iris_synthetic_data.csv](iris_synthetic_data.csv)

**Project Summary**
This project demonstrates a typical ML workflow for the Iris dataset: data loading, cleaning, visualization, dimensionality reduction (PCA), and training simple classifiers (Logistic Regression, KNN, SVM). The notebook documents EDA steps (correlation heatmaps, PCA plots), model training, and model comparison via accuracy and confusion matrices.

**Files**
- [iris data analysis.ipynb](iris data analysis.ipynb): Jupyter Notebook with code and visualizations.
- [iris_synthetic_data.csv](iris_synthetic_data.csv): Synthetic Iris dataset (csv) used in the notebook.

**Dataset Details**
The CSV includes the following columns:
- `sepal length`, `sepal width`, `petal length`, `petal width` — numeric features
- `sepal area`, `petal area` — computed area features
- `label` — class label (Iris species)

The dataset in this repository contains ~3000 rows (synthetic expansion of the classic Iris dataset).

**How to Use**
1. Create a Python environment (recommended Python 3.9+).

```
python -m venv .venv
# Windows PowerShell
.\.venv\Scripts\Activate.ps1
```

2. Install required packages (suggested):

```
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Launch Jupyter and open the notebook:

```
jupyter notebook "iris data analysis.ipynb"
```

4. Run the notebook cells in order. The notebook reads the dataset from `iris_synthetic_data.csv` (assumes both files are in the same folder).

**Key Notebook Steps**
- Data loading and basic checks: `df.info()`, `df.describe()`, missing values and duplicates checks.
- Correlation heatmap and dropping highly correlated columns (`sepal area`, `petal area`).
- Feature scaling and PCA visualization (2 components).
- Train/test split and training of Logistic Regression, KNN, and SVM.
- Visualization of confusion matrices and an SVM decision boundary for two features.

**Dependencies**
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Consider pinning versions in a `requirements.txt` for reproducibility.

**Results**
Model accuracies are printed in the notebook for Logistic Regression, KNN, and SVM. Use the notebook to reproduce the numeric results and plots.

**Next Steps / Suggestions**
- Add `requirements.txt` with pinned versions.
- Add a short script to run automated evaluation (e.g., `evaluate.py`).
- Add unit tests for data loading and preprocessing steps.
- Optionally split dataset creation/generation code into a separate script if you regenerate synthetic data.

**License**
This repository is unlicensed. Add a license file if you intend to publish it publicly (MIT recommended for permissive use).

**Contact / Author**
If you want edits or a different README tone (academic, portfolio, or tutorial), tell me and I will update it.
