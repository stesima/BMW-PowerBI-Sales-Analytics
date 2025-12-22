# 🏛️ BMW Global Sales Analytics – Power BI Dashboard

## 📌 Project Overview  
This project presents an end-to-end **Power BI analytics solution** designed to explore and summarize **BMW global sales performance** over the period **2010–2024**.

The objective of the project is not to replicate real BMW results, but to **demonstrate a complete and professional Business Intelligence workflow**, including data preparation, modeling, DAX development, and dashboard design, following enterprise-level best practices.

The final output consists of **six interactive dashboards**, each focused on a specific business perspective: overall performance, regional dynamics, product mix, pricing behavior, electrification trends, and scenario-based forecasting.

---

## 🗂️ Dataset Description  
- **Source:** Kaggle  
- **Type:** Synthetic dataset (not real BMW data)  
- **Time span:** 2010–2024  
- **Granularity:** Annual, aggregated by model and region  

The dataset includes sales volumes, prices, revenue, model attributes, regions, fuel types, and technical characteristics.

---

## 🧹 Data Preparation & Feature Engineering  
Data preparation was performed in **Power Query**, including:
- Validation and standardization of numerical and categorical variables  
- Creation of derived metrics, including **Revenue = Units × Price**  
- Transformation of continuous variables into analytical bands (price, mileage, engine size)  
- Grouping of individual models into **Model Families** for portfolio-level analysis  
- Custom sort columns to ensure correct ordering in visuals  

All transformations were applied before loading data into the Power BI model.

---

## 🧩 Data Modeling Approach  
The data model follows a **simplified star-schema logic**:
- One central fact table containing sales and descriptive attributes  
- A dedicated **YearTable** created in DAX to manage time-based analysis  

The model operates at annual granularity, ensuring stable slicer behavior and reliable time intelligence calculations such as YoY growth and CAGR.

---

## 📐 DAX Measures & Analytical Logic  
The dashboard is powered by a structured set of reusable DAX measures, including:
- **Total Revenue, Total Units, ASP**
- Revenue, Units, and ASP **Year-over-Year (%) and Δ**
- Revenue Share and CAGR
- **What-if scenario measures** for price and volume growth  

All measures are designed to be robust to filters and consistently reused across dashboards.

---

## 📊 Dashboard Pages & Key Insights  

### 1️⃣ Performance Overview  
Executive-level view of global performance, highlighting overall revenue, units, ASP, and long-term trends.

### 2️⃣ Regional Performance  
Comparison of revenue, units, and ASP across regions, with parallel trends and balanced regional contributions.

### 3️⃣ Product & Model Mix  
Analysis of model families, fuel types, and price bands, showing portfolio composition and revenue concentration by segment.

### 4️⃣ Pricing & Profitability  
Focus on ASP dynamics, revenue per unit, and pricing stability across models and over time.

### 5️⃣ Electrification & Sustainability  
Overview of electric and alternative powertrain adoption, tracking units share, revenue share, and ASP evolution.

### 6️⃣ Forecast & Scenario Analysis  
Interactive what-if analysis allowing users to simulate price and volume growth scenarios and compare base vs scenario outcomes.

---

## 📸 Sample Dashboard – Product & Model Mix

![Control Chart](assets/Product_Dashboard.png)

This dashboard provides a portfolio-level view of BMW’s **product and model composition**, combining sales volumes, pricing metrics, and segmentation logic in a single analytical view.

It highlights how different **model families** contribute to total units, how **fuel types** are distributed across the portfolio, and how **revenue concentrates across price bands**. The combination of stacked bars and ASP trends enables a joint analysis of **volume structure and pricing stability over time**.

Although the underlying dataset is synthetic and shows limited variability, the dashboard reflects a **realistic analytical layout** commonly used in automotive portfolio analysis, emphasizing clarity, consistency, and executive-oriented storytelling.

---

## ⚠️ Data Limitations & Interpretation  
This project is based on a **synthetic dataset**, not on real BMW sales data.

Key limitations include:
- Uniform and symmetrical distributions across key variables  
- Balanced representation of regions, models, and fuel types  
- Simplified relationships between price, volume, and technical attributes  

As a result, some visualizations may appear **flat or homogeneous**, with limited differentiation across segments.  
These limitations are inherent to the dataset and **do not reflect shortcomings in data modeling, DAX logic, or dashboard design**.

Insights should therefore be interpreted as **relative comparisons**, not as real market conclusions.

---

## 🛠️ Technologies & Skills Demonstrated  
- Power BI  
- Power Query (data cleaning and transformation)  
- DAX (time intelligence, advanced measures, what-if analysis)  
- Data modeling (star schema, filter management)  
- Dashboard design and analytical storytelling


---

## 📁 Project Structure

The repository is organized to clearly separate data sources, Power BI files, and visual assets, following a clean and scalable project structure.
```bash
BMW-PowerBI-Sales-Analytics/
│
├── README.md # Project overview and documentation
├── LICENSE # MIT License
│
├── data/
│ └── BMW sales data (2010-2024).csv # Source dataset (synthetic, Kaggle)
│
├── powerbi/
│ └── BMW Dashboards.pbix # Power BI dashboard file
│
├── assets/
│ └── Report.pdf
│ └── Product_Dashboard.png
│ # Dashboard preview used in README
```
---

## 🎯 Project Purpose  
The primary goal of this project is to **demonstrate professional Business Intelligence and analytics skills**, showcasing the ability to build clean data models, develop robust DAX measures, and design executive-ready dashboards while transparently addressing data limitations.

---

## 📫 Contact
**Author**: Stefano Sima  

- 📧 Email: [stefano.sima@mail.polimi.it](mailto:stefano.sima@mail.polimi.it)  
- 💼 LinkedIn: [linkedin.com/in/stesima](https://www.linkedin.com/in/stesima)  
