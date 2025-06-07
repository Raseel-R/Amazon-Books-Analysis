# 📚 Amazon-Books-Analysis Data Science Project

A complete data science pipeline using web-scraped data from Amazon book listings. The project covers data cleaning, feature encoding, exploratory data analysis, and building regression models to predict book ratings.

---

## 🌐 Data Source

- Web-scraped book data from Amazon.com
- Key features: Book Name, Author, Rating, Price, Number of Reviews, Format, Other Format

---

## 🧹 Data Cleaning & Preparation

- Removed missing/invalid entries (e.g., Prime Video, None)
- Cleaned `Rating` and `Author` columns (e.g., removed "by", stripped strings)
- Removed duplicate book entries
- Applied **Label Encoding** on `Format` and `Other Format` columns
- Converted features to appropriate data types for analysis

---

## 🔍 Exploratory Data Analysis (EDA)

- Calculated skewness of all numerical features
- Visualized distributions using histograms and boxplots
- Answered key questions:
  - 📘 Which book format has the highest average rating? → Paperback, Hardcover, Board Book
  - 💰 What’s the correlation between price and rating? → Weak negative correlation (≈ -0.1)
  - ✍️ Which author appears most? → Determined using `.mode()`

---

## 🤖 Predictive Modeling

Goal: Predict book ratings using regression algorithms

### Models Evaluated:
- **Linear Regression**
- **Random Forest Regression**
- **Gradient Boosting Regression**
- **Baseline Mean Model**

### Evaluation Metrics:
- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)

### Results:
- ✅ **Linear Regression** performed best overall:
  - RMSE: 0.310
  - MAE: 0.256

---

## 🛠 Tools & Technologies

- Python, Jupyter Notebook  
- pandas, matplotlib, seaborn  
- scikit-learn (LabelEncoder, Regression models)

---

## 🎯 Project Purpose

Developed to demonstrate practical data science skills:
- Real-world web scraping
- Data bias detection
- EDA and visualization
- Model building and performance comparison
