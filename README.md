# mist4610-project2-group-7

## Team Name:
15058 Group 7

## Team Members:
1. Tyler Schildkraut [@tylerschildkraut](https://github.com/tylerschildkraut)
2. Angela Ren [@angelaaa456](https://github.com/angelaaa456)
3. Sammy Effron [@seffron](https://github.com/seffron)
4. Audrey Staples [@audreystaples](https://github.com/audreystaples)
5. Tanner Sutherland [@tannersutherland](https://github.com/tannersutherland)

# Dataset Description

### **Dataset Title:**  
**Real Estate Sales 2001–2023 GL** (from data.gov)

### **Dataset Scope:**  
State of Connecticut real estate sales records.

### **Why We Chose This Dataset**  
The housing market is a powerful indicator of economic health, and the dataset contains intuitive, real-world variables that translate directly into insights. It is also extremely rich:  
- **1,142,722 rows**  
- **14 columns**  
- Covers all Connecticut towns and multiple property types  
:contentReference[oaicite:1]{index=1}

### **Key Variables Used**
- **Serial Number** – Unique property ID  
- **List Year** – Year the property was listed  
- **Town** – Town name  
- **Address** – Street address  
- **Assessed Value** – Tax assessed property value  
- **Sale Amount** – Actual sale price  
- **Sales Ratio** – *Assessed Value / Sale Amount*  
  - < 1.00 → Under-assessed  
  - > 1.00 → Over-assessed  
- **Property Type** – Residential, Commercial, Industrial, etc.  
- **Residential Type** – Single-family, Condo, etc.  

### **Variables Excluded (and why)**
- Date Recorded, Non-Use Code, Assessor Remarks, OPM Remarks, Location  
**Reasons**: redundant, low insight, or not intuitive.  

# Research Questions

## **Question 1 (Analytical)**
**How did average prices across Connecticut towns change from 2018–2023, especially during and after the COVID-19 housing surge?**


# Data Manipulation for Question 1
- Computed average sale amounts per town per year  
- Calculated % growth from 2018–2023  
- Identified **top 10 fastest-growing towns**  
- Created:
  - Box & whisker distribution plot  
  - Bar chart of top growth towns  
  - Line chart of YOY change  
  - Pre-COVID and Post-COVID price heat maps  

# **Visualizations for Question 1**

### **Statewide Distribution — Box & Whisker Plot**
![Box Plot – Price Growth Distribution](graphs/Question1_Boxwhiskerplot.png)

### **Top 10 Towns — Price Growth (Bar Chart)**
![Top 10 Towns Price Growth](graphs/Question1_Graph1.png)

### **Year-over-Year Average Sale Amounts (Line Chart)**
![YOY Average Sale Amount](graphs/Question1_Graph2.png)

### **Average Sale Prices Per Town — Pre-COVID**
![Pre-COVID Average Price Map](graphs/Question1_Graph3.png)

### **Average Sale Prices Per Town — Post-COVID**
![Post-COVID Average Price Map](graphs/Question1_Graph4.png)

# **Analysis for Question 1**

- Home prices rose sharply from **2018–2023**, with the most pronounced increases occurring from **2020–2022** during the COVID housing surge.  
- The **median Connecticut town** saw **40–50% growth**.  
- Most towns clustered between **20–70% growth**, while a smaller set surged **150–325%**, highlighting major regional disparities.  
- Lower-priced towns exhibited the largest percent gains (low base values + high COVID migration).  
- Higher-priced towns showed strong absolute dollar growth but smaller percentage increases.  
- By 2023, markets diverged: some cooled while others continued trending upward.

# **Question 2 (Explanatory)**  
**On average, have assessed values kept pace with actual sale prices from 2018–2023, and which property types show the largest valuation gaps?**


# Data Manipulation for Question 2
- Aggregated **median assessed values** by property type  
- Calculated **median actual sale prices** by property type  
- Computed **sales ratios** (Assessed ÷ Sale Price)  
- Mapped sales ratios for:
  - Commercial properties  
  - Residential properties  

# **Visualizations for Question 2**

### **Median Assessed Value by Property Type**
![Assessed Values – Property Types](graphs/Question2_Graph1.png)

### **Median Actual Sale Price by Property Type**
![Sale Amounts – Property Types](graphs/Question2_Graph2.png)

### **Commercial Sales Ratio Map**
![Commercial Sales Ratio Map](graphs/Question2_Graph3.png)

### **Residential Sales Ratio Map**
![Residential Sales Ratio Map](graphs/Question2_Graph4.png)


# **Analysis for Question 2**

- **Assessed values did not keep pace** with actual transaction prices from 2018–2023.  
- Nearly all property types were **under-assessed**, with sale prices significantly higher than assessments.  
- **Industrial properties** showed the **largest undervaluation** (~$300K gap).  
- **Apartments** had assessed values at roughly **half** of actual sales prices.  
- **Public utility** was the only over-assessed outlier.  
- Mapping showed widespread under-assessment, especially for residential properties during the COVID price surge.

# Final Summary

- Connecticut home prices rose significantly between 2018–2023, with extreme spikes during COVID  
- Growth was highly uneven—some towns soared 3–6× beyond the median  
- Post-COVID trends diverged (cooling vs. continuing acceleration)  
- Assessed values lagged far behind sale prices in almost every property category  
- Residential and industrial assets were most undervalued  
- Overall, COVID, remote work trends, and regional migration reshaped Connecticut’s housing market  


# **Honors Option — Predictive Analysis (Question 3)**  
*(Completed individually by Tyler Schildkraut for Honors Credit)*

## Predictive Question  
**“Based on year-over-year sales volume trends, which Connecticut towns are likely to have increasing housing demand in the next year?”**

# Visualization — Forecasted Sales Volume (2018–2025)

![Forecasted Sales Volume](graphs/Question3_Graph1.png)

# Methodology (Predictive)

- Identified the **top 10 towns by total sales volume** (2018–2023).  
- Built a **year-over-year line chart** of annual transaction counts.  
- Applied Tableau’s **Forecast (Exponential Smoothing)** model to project sales for:
  - **2024**
  - **2025**

Forecast captures:
- Trend  
- Volatility  
- Momentum  

# Key Forecast Findings

### **Towns with Increasing Demand (Upward Forecast)**  
#### **Stamford**
- Strong recovery after 2022  
- Projected renewed growth  
- Consistently one of CT’s highest-volume markets  

#### **Bridgeport**
- Forecast shows continued upward trend  
- High activity even during post-COVID cooling  

#### **Waterbury**
- Upward momentum in recent data  
- Forecast suggests continued stability + growth  

### **Towns with Stable or Cooling Demand (Flat/Downward Forecast)**

#### **Hamden**
- Flat-to-declining forecast  
- Lower volume than major cities  

#### **New Haven**
- Forecast indicates leveling off  
- Slight decline after 2021 peak  

#### **West Hartford**
- Clear downward slope in forecast  
- Strongest indicator of cooling end-user demand  

#  Why This Predictive Question Matters

Sales **volume** signals **true underlying buyer activity**, making it a powerful predictor of future competitiveness.  
Unlike price-based metrics, volume shows how frequently properties transact — reflecting demand strength, affordability, and market liquidity.

# Predictive Summary

- Stamford, Bridgeport, and Waterbury expected to see **increasing activity** in 2024–2025.  
- Hamden, New Haven, and West Hartford show **cooling or stabilizing** demand.  
- The forecast reveals diverging post-COVID trajectories among Connecticut’s highest-activity towns.  
