# Product-Segementation

\# 🛒 Product Segmentation in E-commerce using Unsupervised Learning



\## 📌 Project Overview



This project focuses on segmenting e-commerce products based on pricing and discount behavior using unsupervised learning techniques. The goal is to identify meaningful product groups that can help businesses understand pricing strategies and customer targeting.



\---



\## 🎯 Objective



\* Perform product segmentation using clustering techniques

\* Identify patterns in pricing and discount behavior

\* Generate actionable business insights from clusters



\---



\## 📊 Dataset



\* Source: Flipkart Products Dataset (Kaggle)

\* Size: \~20,000 products

\* Features used:



&#x20; \* `retail\_price`

&#x20; \* `discounted\_price`

&#x20; \* `product\_category\_tree`

&#x20; \* `brand`



\---



\## 🧹 Data Preprocessing



\* Removed irrelevant columns (IDs, URLs, timestamps, etc.)

\* Handled missing values in price columns

\* Removed extreme outliers in pricing

\* Converted data types where necessary



\---



\## ⚙️ Feature Engineering



\* Created `discount\_percent` to capture pricing strategy

\* Applied log transformation (`price\_log`) to handle skewed price distribution

\* Extracted `Main\_Category` from hierarchical category data

\* Created `is\_branded` feature for analysis



\---



\## 🤖 Modeling Approach



\* Standardized features using `StandardScaler`

\* Applied \*\*K-Means Clustering\*\*

\* Used \*\*Elbow Method\*\* to determine optimal number of clusters (k=3)



\---



\## 📊 Cluster Interpretation



\* \*\*Cluster 2\*\* represents premium, high-priced products with minimal discounting

\* \*\*Cluster 1\*\* represents discount-driven products with aggressive pricing strategies

\* \*\*Cluster 0\*\* represents regular products with moderate pricing and discount levels



\---



\## 📈 Key Insights



\* Premium products are heavily brand-driven (\~95% branded)

\* Discount-driven products dominate the dataset, highlighting price sensitivity

\* Regular segment contains a mix of branded and local products

\* Clothing is the dominant category across all segments



\---



\## 🧪 Feature Experiment (Important)



An experiment was conducted by including the `is\_branded` feature in clustering:



\* Result: Clusters became dominated by brand presence

\* Impact: Reduced effectiveness of price-based segmentation



👉 Conclusion:

`is\_branded` was excluded from clustering and used only for post-analysis.



\---



\## 📊 Visualizations



\* Cluster distribution (bar chart)

\* Price distribution across clusters (boxplot)

\* Discount distribution across clusters (boxplot)

\* Scatter plot of clustered data



\---



\## 🛠️ Tech Stack



\* Python

\* Pandas, NumPy

\* Matplotlib, Seaborn

\* Scikit-learn



\---



\## 🚀 Conclusion



This project demonstrates how unsupervised learning can be used to uncover meaningful product segments in e-commerce. By focusing on pricing and discount patterns, businesses can better understand market dynamics and optimize strategies.



\---

