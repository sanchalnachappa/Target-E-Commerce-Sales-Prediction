# Target E-Commerce Sales Prediction
Data Science and Business Analytics Project  
McCombs School of Business, The University of Texas at Austin

![Target E-Commerce Sales Analysis](Sales_forecasting.png)

---

## Project Overview
This project analyzes and forecasts daily e-commerce sales for Target’s operations in Brazil between 2016 and 2018.  
The goal was to develop a reproducible forecasting model and generate business insights that could support operational planning, regional stocking, and marketing strategies.  

The analysis covers order activity, customer behavior, payment methods, logistics performance, and geographic patterns, integrating multiple data sources into a unified analytical framework.

---

## Dataset Description
The dataset contains about 100,000 orders and is divided across eight relational tables: customers, sellers, order items, geolocation, payments, orders, and products.  
Each record includes detailed information on order status, pricing, payment method, shipping performance, customer location, product attributes, and reviews.

**Primary business questions**
1. Can daily sales be forecast accurately?  
2. Can the forecasts improve operational planning?  
3. Can a scalable, reproducible model be developed for broader business use?

---

## Importance of the Problem
E-commerce companies rely heavily on accurate forecasting and segmentation to maintain profitability and customer satisfaction.  
The insights from this project can be applied to:
- Improve demand planning and inventory allocation by region  
- Guide digital marketing and promotional timing  
- Increase profitability through customer segmentation and retention analytics  
- Create scalable modeling workflows adaptable to larger datasets and new sources  

---

## Exploratory Data Analysis
The exploratory phase focused on cleaning, merging, and visualizing multiple data sources.

**Key steps**
- **Relevance filtering:** kept only variables aligned with forecasting objectives  
- **Data merging:** combined eight feature tables into one analytical dataset  
- **Geographic mapping:** visualized orders, calculated distances, and identified regional buying patterns  
- **Standardization:** corrected column names, fixed date formats, handled missing values  

**Notable findings**
- Clear seasonal peaks in November sales, driven by holiday campaigns  
- Rolling 7-day averages revealed short-term demand momentum  
- Daily sales statistics: mean ≈ $20.7 K  |  median ≈ $20.5 K  |  maximum ≈ $179.2 K  

---

## Modeling and Evaluation
Four models were tested: Naïve, Seasonal Naïve, Linear Regression, and Gradient Boosting.  
Model performance was evaluated using MAE, RMSE, sMAPE, and WAPE.  

**Best-performing model:** Linear Regression  
- MAE = $6,102  
- RMSE = $7,265  

Despite its simplicity, the linear model achieved the strongest accuracy and generalization.  
This indicates that a small set of well-chosen time and category features captured most of the sales variation in the dataset.

---

## Insights and Business Implications
- **Seasonality:** pronounced November sales peaks suggest strong responsiveness to promotions and holidays.  
- **Regional trends:** geographic differences point to the need for region-specific stocking and marketing approaches.  
- **Customer segmentation:** RFM analysis (Recency, Frequency, Monetary) identified customer clusters for retention and upsell targeting.  
- **Forecasting utility:** daily predictions from the linear model can guide short-term inventory and logistics planning.  
- **Scalability:** the framework can be extended to include additional signals such as product reviews, browsing data, or campaign metadata.  

Integrating these models into operational dashboards (Excel or Power BI) enables cross-departmental access and faster decision-making.

---

## Technologies Used
Python (NumPy, Pandas, Matplotlib, Scikit-learn), Power BI, Jupyter Notebook



| File | Description |
|------|--------------|
| [Daily_sales_forecasting.pdf](Daily_sales_forecasting.pdf) | Full written report including methodology, metrics, and recommendations |
| [Sales_forecasting_ppt.pdf](Sales_forecasting_ppt.pdf) | Executive presentation summarizing findings |
| [Sales_Prediction_with_o_p.ipynb](Sales_Prediction_with_o_p.ipynb) | Jupyter notebook with preprocessing, EDA, and modeling code |


---

## Conclusion
The project demonstrates that a transparent, interpretable model such as linear regression can deliver highly reliable daily sales forecasts for an e-commerce platform.  
Beyond forecasting accuracy, the analysis highlights actionable insights into regional buying patterns, customer behavior, and campaign timing each directly applicable to business planning and profitability improvement.

---

## Contact
For further discussion or access to supplementary materials, please reach out via  
[LinkedIn – Suryah Vadivel](https://www.linkedin.com/in/suryahvadivel)
