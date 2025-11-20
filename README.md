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
:contentReference[oaicite:2]{index=2}

### **Variables Excluded (and why)**
- Date Recorded, Non-Use Code, Assessor Remarks, OPM Remarks, Location  
**Reasons**: redundant, low insight, or not intuitive.  
:contentReference[oaicite:3]{index=3}

# Research Questions

## **Question 1 (Analytical):**
**How did average prices across Connecticut towns change from 2018–2023, especially during and after the COVID-19 housing surge?**  
:contentReference[oaicite:4]{index=4}

### **Why it’s important**
- Housing prices reflect macroeconomic health  
- COVID-era migration heavily affected suburban markets  
- Identifies which towns surged vs. stagnated  
- Shows the timing and impact of pandemic-driven demand

---

## **Question 2 (Explanatory):**
**Have assessed values kept pace with actual sale prices from 2018–2023, and which property types show the largest valuation gaps?**  
:contentReference[oaicite:5]{index=5}

### **Why it’s important**
- Assessed values affect taxes & municipal budgets  
- Under-assessment indicates outdated valuations  
- Helps reveal which markets changed fastest  
- Highlights potential policy or fiscal implications

---

# Data Manipulations (Tableau)

### **For Question 1: Price Growth by Town**
- Created a distribution plot showing % growth across all 169 towns  
- Calculated average sale amounts by year for each town  
- Filtered down to **Top 10 fastest-growing towns** for clarity  
- Generated line charts for year-over-year price trends  
:contentReference[oaicite:6]{index=6}

### **For Question 1: Pre- vs. Post-COVID**
- Split dataset into:
  - **Pre-COVID:** 2018–early 2020  
  - **Post-COVID:** 2020–2023  
- Mapped average sale prices for each town in both periods  
- Compared spatial/geographic price patterns  

### **For Question 2: Assessed Value vs. Sale Price**
- Calculated median assessed and sale prices by property type  
- Built comparative bar charts by:
  - Apartments  
  - Commercial  
  - Condo  
  - Industrial  
  - Residential / Single-Family  
  - Vacant Land  
- Computed sales ratios to reveal under- vs over-valuation by town  
- Created separate maps of commercial and residential sales ratios  

# Analysis & Results

## **Results for Question 1: How did prices change from 2018–2023?**
- Home prices **rose sharply statewide**, with fastest acceleration from **2020–2022**  
- Median CT town grew **~40–50%**  
- Most towns clustered between **20%–70%** growth  
- **Top 10 towns** surged **150–325%**, driven by:
  - Low starting prices  
  - COVID-era in-migration  
  - Limited inventory  
- Higher-priced towns saw strong dollar increases but lower percent gains  
- In 2023, markets diverged: some cooled, others kept rising  

**Key takeaway:**  
COVID amplified disparities—some CT towns exploded in growth while others followed moderate statewide trends.


## **Results for Question 2: Do assessed values keep up with sale prices?**
- **Assessments did NOT keep pace with actual sale prices** from 2018–2023  
- Sale prices were higher than assessed values across almost all property types  
- Largest undervaluations:
  - **Industrial** (≈ $300K undervalued)  
  - **Apartments** (≈ double assessed value)  
- Only outlier: **Public Utility** (assessed > sale price)  
- Maps show nearly all towns in deep red (sales ratio < 1), especially for residential  

**Key takeaway:**  
Nearly all CT towns under-assessed properties—especially residential and industrial—because assessments lagged behind rapid market price increases.


# Final Summary

- Connecticut home prices rose significantly between 2018–2023, with extreme spikes during COVID  
- Growth was highly uneven—some towns soared 3–6× beyond the median  
- Post-COVID trends diverged (cooling vs. continuing acceleration)  
- Assessed values lagged far behind sale prices in almost every property category  
- Residential and industrial assets were most undervalued  
- Overall, COVID, remote work trends, and regional migration reshaped Connecticut’s housing market  


