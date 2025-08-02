# 📊 Market Campaign Report – Power BI

## 📌 Overview
This project is part of my internship at **Future Interns**.  
The goal was to design and build an **interactive Power BI dashboard** that analyzes marketing campaign performance and provides actionable insights for decision-makers.

The dashboard helps marketing teams:
- Identify **high-value customers**
- Understand **campaign effectiveness**
- Explore **spending patterns by demographics**
- Discover **top-performing markets**

---

## 🚀 Key Insights
- 💰 **$1.36M** total campaign spend
- 👥 **2,240** customers analyzed
- 🏆 **918** high-value customers identified
- 📈 Campaign 3 & Campaign 5 have the highest acceptance rates
- 🎓 Graduates contribute the largest share of revenue
- 🌍 Spain is the top-spending country

---

## 🛠 Tools & Skills Used
- **Power BI** – Data modeling, DAX measures, interactive visuals
- **Power Query** – Data cleaning & transformation
- **Excel** – Data inspection & initial formatting
- **Business Analysis** – Aligning insights with marketing goals

---

## 📂 Dataset
The dataset contains:
- **Customer demographics** – Age, education, marital status, income, country
- **Purchase data** – Amount spent on different product categories
- **Campaign data** – Responses to marketing campaigns
- **Engagement metrics** – Web visits, purchases via different channels

---

## 🔍 Key Calculations
Some of the calculated measures used in the report:
```DAX
Age = YEAR(TODAY()) - 'marketing_data'[Year_Birth]

Total Spend =
    'marketing_data'[MntWines] +
    'marketing_data'[MntFruits] +
    'marketing_data'[MntMeatProducts] +
    'marketing_data'[MntFishProducts] +
    'marketing_data'[MntSweetProducts] +
    'marketing_data'[MntGoldProds]

High Value Customer =
    IF([Total Spend] > AVERAGE('marketing_data'[Total Spend]), "Yes", "No")

Age = YEAR(TODAY()) - 'marketing_data'[Year_Birth]

Total Spend =
    'marketing_data'[MntWines] +
    'marketing_data'[MntFruits] +
    'marketing_data'[MntMeatProducts] +
    'marketing_data'[MntFishProducts] +
    'marketing_data'[MntSweetProducts] +
    'marketing_data'[MntGoldProds]

High Value Customer =
    IF([Total Spend] > AVERAGE('marketing_data'[Total Spend]), "Yes", "No")

![snippet](https://github.com/user-attachments/assets/2bb60cd1-b462-4e51-9ad2-3ee778898b77)
