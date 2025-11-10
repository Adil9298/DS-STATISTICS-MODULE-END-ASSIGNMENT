# 📊 Customer Purchase & Churn Analysis – Statistics Project

This project performs a complete statistical analysis on a retail customer dataset to understand purchasing behavior, churn patterns, and the effectiveness of marketing campaigns.  
It is implemented in **Python**, using **Google Colab** for data analysis and visualization.

---

## ✅ **Project Objectives**

The goal of the assignment is to analyze customer behavior using statistical and mathematical tools, and answer the following questions:

1. What is the **average, median, and mode** of PurchaseAmount?
2. Are there any **outliers** in the data?
3. What are the **skewness and kurtosis** values of the PurchaseAmount distribution?
4. Is there a significant difference in spending between **male vs female** customers?
5. Is there a relationship between **ProductCategory** and **Churn**?
6. Does PurchaseAmount vary significantly across **regions**?
7. Which marketing **email campaign group (A/B)** performs better?
8. Does PurchaseAmount follow a **normal distribution**?
9. What insights can be gained from the **Central Limit Theorem (CLT)**?
10. What is the **95% confidence interval** for the population mean PurchaseAmount?

---

## ✅ **Dataset Details**

The dataset contains the following columns:

| Column Name        | Description |
|-------------------|-------------|
| CustomerID        | Unique customer identifier |
| Gender            | Male / Female |
| Region            | North / South / East / West |
| PurchaseAmount    | Total purchase value |
| ProductCategory   | Fashion / Grocery / Electronics |
| Churn             | Indicates if customer churned (Yes/No) |
| CampaignGroup     | Marketing campaign group (A/B) |

You can upload the CSV file manually into **Google Colab**.

---

## ✅ **Technologies Used**

- Python  
- Google Colab  
- pandas  
- numpy  
- scipy  
- matplotlib  

---

## ✅ **How to Run the Notebook (Google Colab)**

### **1️⃣ Install dependencies**

```python
!pip -q install pandas scipy matplotlib
```


### **2️⃣ Upload the dataset manually**

```python
from google.colab import files
uploaded = files.upload()

file_name = next(iter(uploaded))
df = pd.read_csv(file_name)
df.head()
```

### **3️⃣ Perform all statistical analysis**

The notebook includes:

✅ Mean, Median, Mode
✅ Outlier detection (IQR method)
✅ Skewness & Kurtosis
✅ Welch’s t-test (Male vs Female)
✅ Chi-square test (ProductCategory vs Churn)
✅ ANOVA + Kruskal test (Regions)
✅ Campaign comparison (A vs B)
✅ Normality test + Q–Q plot
✅ CLT simulation plots
✅ 95% Confidence Interval

All visualizations (Histogram, Boxplot, and CLT plots) are generated automatically.

✅ Key Statistical Results (Summary)
Metric	Value
Mean PurchaseAmount	~1029.50
Median	~1021.96
Skewness	Slight left skew
Kurtosis	Platykurtic (flatter than normal)
Campaign Winner	Campaign B
Male vs Female Spending	Females spend more
95% CI for mean	(866.79, 1192.21)
Regional effect	No significant difference (p > 0.05)

✅ Conclusion

This project demonstrates:

Practical use of statistical testing

Understanding of distribution analysis

Application of Central Limit Theorem

Real-world comparison of marketing campaign performance

Confidence interval estimation for business insights

✅ Author

MOHAMMED ADIL. K
Data Science & Machine Learning
