# Data-Analysis-with-Jupyter-Notebook

# Iris Dataset Analysis

This project performs data exploration and visualization on the classic [Iris flower dataset](https://archive.ics.uci.edu/ml/datasets/iris), which contains measurements of 150 iris flowers from three species: *setosa*, *versicolor*, and *virginica*.

---

## 📊 Dataset Overview

The dataset consists of 150 rows and the following 5 columns:

- `sepal_length` (in cm)
- `sepal_width` (in cm)
- `petal_length` (in cm)
- `petal_width` (in cm)
- `class` (species: Setosa, Versicolor, Virginica)

---

## 🔍 Data Exploration

- Used `df.info()` and `df.isnull().sum()` to inspect structure and missing values.
- Verified that no missing values exist in the dataset.
- Displayed basic statistics using `.describe()` and `.median()`.

---

## 🧼 Data Cleaning

While the dataset was already clean, the following steps are included for general practice:

- `df.dropna()` – to drop missing rows
- `df.fillna(df.mean())` – to fill missing values with column means

---

## 📈 Visualizations

Four visualizations were created using **Matplotlib** and **Seaborn**:

1. **Line Chart** – Trend of petal length across sample index (simulated time series)
2. **Bar Chart** – Average petal length grouped by species
3. **Histogram** – Distribution of sepal width
4. **Scatter Plot** – Relationship between sepal length and petal length, colored by species

Each plot includes titles, axis labels, and legends where appropriate.

---

## 🧠 Insights

- *Setosa* flowers have much shorter petals than the other species.
- *Virginica* tends to have the largest feature measurements.
- *Versicolor* features lie between the other two species.
- Petal dimensions are more effective for distinguishing species than sepal dimensions.

---

## 🛠 Tools Used

- Python
- Pandas
- Matplotlib
- Seaborn

---

## 📦 Requirements

Install the required Python packages using `pip`:

```bash
pip install pandas matplotlib seaborn
