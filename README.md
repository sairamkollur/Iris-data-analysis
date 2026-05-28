# 🌸 Task 3 – Exploratory Data Analysis (EDA) on Iris Dataset

**Edutech Solution AI & ML Internship — Task 3**

---

## 📌 Objective

Perform a full Exploratory Data Analysis (EDA) on the classic **Iris Dataset** using Python. The goal is to extract meaningful insights through statistical summaries and visualizations before any modelling step.

---

## 📂 Project Structure

```
Iris-data-analysis/
│
├── Iris.csv                    # Dataset (150 rows × 6 columns)
├── iris_eda.ipynb              # Main Jupyter Notebook with full EDA
├── requirements.txt            # Python dependencies
└── README.md                   # This file
```

---

## 📊 Dataset Overview

| Feature         | Description                        |
|----------------|------------------------------------|
| `SepalLengthCm` | Sepal length in centimetres        |
| `SepalWidthCm`  | Sepal width in centimetres         |
| `PetalLengthCm` | Petal length in centimetres        |
| `PetalWidthCm`  | Petal width in centimetres         |
| `Species`       | Iris-setosa / versicolor / virginica |

- **150 samples**, 3 classes (50 each), no missing values.

---

## 🔍 EDA Steps Covered

### 1. Univariate Analysis
- Histograms for all numerical features
- Box plots per feature (with and without species grouping)
- Statistical summaries (mean, std, min/max, quartiles)

### 2. Bivariate Analysis
- Scatter plots between feature pairs, coloured by species
- Bar charts of mean feature values per species
- Violin plots for distribution shape per class

### 3. Correlation Matrix & Heatmap
- Pearson correlation matrix for numerical features
- Annotated heatmap to visualise multicollinearity

### 4. Multivariate Analysis
- Pair plot across all four numerical features
- Colour-coded by species for cluster visibility

### 5. Outlier Detection
- Box plots to visually spot outliers (IQR method)

### 6. Key Insights Summary
- Petal features are stronger discriminators than sepal features
- Iris-setosa is linearly separable from the other two species
- Petal Length and Petal Width are highly correlated (r ≈ 0.96)
- Sepal Width shows the most overlap between versicolor and virginica

---

## 🚀 Setup & Run

### 1. Clone the repository
```bash
git clone https://github.com/sairamkollur/Iris-data-analysis.git
cd Iris-data-analysis
```

### 2. Create and activate a virtual environment

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**macOS / Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook iris_eda.ipynb
```

---

## 🧠 Interview Questions & Answers

**Q: What is the difference between Univariate, Bivariate, and Multivariate analysis?**  
- **Univariate** – analysis of a single variable (e.g. histogram of Petal Length).  
- **Bivariate** – relationship between two variables (e.g. scatter plot of Sepal vs. Petal).  
- **Multivariate** – simultaneous analysis of three or more variables (e.g. pair plot coloured by species).

**Q: How do you interpret a Correlation Heatmap?**  
Values close to **+1** indicate strong positive correlation; close to **−1** indicate strong negative correlation; near **0** means little to no linear relationship. Darker or brighter cells (depending on colour scheme) highlight the strongest pairs.

**Q: What is the purpose of a Box plot?**  
Box plots visualise the five-number summary (min, Q1, median, Q3, max) and flag potential outliers as individual points beyond the whiskers.

**Q: How do you identify outliers visually?**  
Data points plotted beyond the box-plot whiskers (1.5 × IQR above Q3 or below Q1) are considered potential outliers.

**Q: Why is EDA the most important step before modelling?**  
EDA reveals data quality issues (missing values, wrong types), the distribution of features, class imbalance, and relationships between variables — all of which inform feature selection, scaling strategy, and model choice.

---

## 🛠 Tools & Libraries

| Tool        | Purpose                          |
|------------|----------------------------------|
| Python 3.x  | Core programming language        |
| Pandas      | Data loading and manipulation    |
| Matplotlib  | Base plotting library            |
| Seaborn     | Statistical visualisations       |
| Jupyter     | Interactive notebook environment |

---

## 📝 License

This project is submitted as part of the **Edutech Solution AI & ML Internship – Task 3**.
