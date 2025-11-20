# mist4610-project2-group-7

## Team Name:
15058 Group 7

## Team Members:
1. Tyler Schildkraut [@tylerschildkraut](https://github.com/tylerschildkraut)
2. Angela Ren [@angelaaa456](https://github.com/angelaaa456)
3. Sammy Effron [@seffron](https://github.com/seffron)
4. Audrey Staples [@audreystaples](https://github.com/audreystaples)
5. Tanner Sutherland [@tannersutherland](https://github.com/tannersutherland)

## Data Set Overview
The dataset used for this project is the “Real Estate Sales 2001–2023 GL” dataset published by the State of Connecticut and made publicly available through data.gov. It contains detailed real estate transaction information across all towns in Connecticut. The dataset consists of 1,142,722 rows and 14 columns, with each row representing an individual property sale. Key fields include Serial Number, List Year, Town, Address, Assessed Value, Sale Amount, Sales Ratio, Property Type, and Residential Type. These fields allow for meaningful analysis of housing market performance, assessment accuracy, and price dynamics across geography and time. Several fields—such as Date Recorded, Non-Use Code, Assessor Remarks, OPM Remarks, and Location—were excluded from analysis because they were redundant, uninformative, or unrelated to the questions explored.

---

## Question 1: Analytical  
**How did average prices across Connecticut towns change from 2018–2023, especially during and after the COVID-19 housing surge?**

This question is important for understanding how Connecticut’s housing market responded to major economic conditions, particularly the unprecedented COVID-19 housing boom. Housing price appreciation reflects broader trends in supply and demand, migration patterns, affordability changes, and macroeconomic pressures. Examining shifts over time and across towns provides insight into which areas experienced the largest surges, how widespread the growth was, and whether the pandemic fundamentally altered local markets.

To answer this question, we calculated the percentage change in average sale amounts for each town between 2018 and 2023. We then identified the top 10 fastest-growing towns and evaluated both statewide patterns and within-town trends. We also produced pre-COVID and post-COVID maps to show how price levels shifted geographically.

### Plot 1: Statewide Price Growth Distribution  
![plot](./Question1_Boxwhiskerplot.png)

**Description and Results:**  
This visualization shows the full distribution of price growth across all 169 Connecticut towns from 2018–2023. The median town grew approximately 40–50%, and most towns fell between 20% and 70%. However, several towns dramatically exceeded statewide norms, with growth between 150% and 325%. These outlier towns indicate extreme market acceleration during the COVID surge, often influenced by low starting prices, sudden in-migration, and increased demand for suburban and rural housing.

### Plot 2: Top 10 Fastest-Growing Towns  
!![plot](./Question1_Graph1.png)

**Description and Results:**  
This bar chart highlights the 10 towns with the highest percentage growth. These towns surged far above the statewide average, experiencing 3–6× the typical appreciation. Many of these towns were lower-priced markets in 2018, making them more sensitive to pandemic-era migration and affordability pressures.

### Plot 3: Year-over-Year Price Trends  
!![plot](./Question1_Graph2.png)

**Description and Results:**  
The year-over-year line chart reveals how each top-growth town evolved during this time period. Some towns experienced steady multi-year increases, while others saw dramatic COVID-era spikes. The strongest acceleration occurred between 2020 and 2022, with 2023 showing mixed outcomes—some markets cooled while others continued rising.

### Plot 4: Pre-COVID Price Map  
!![plot](./Question1_Graph3.png)

### Plot 5: Post-COVID Price Map  
!![plot](./Question1_Graph4.png)

**Description and Results:**  
Comparing these maps shows that before COVID, prices across towns were more balanced. After 2020, nearly all towns saw higher prices, and the gaps between markets widened. Several towns experienced unusually steep growth, while wealthier markets saw more moderate percentage gains.

**Analysis and Helpfulness of Results:**  
Overall, Connecticut experienced substantial price appreciation from 2018–2023, with the most intense increases during COVID. Lower-priced towns appreciated the fastest, consistent with increased demand for affordable housing. Higher-priced towns experienced meaningful dollar increases but smaller percent changes. By 2023, market conditions became more uneven, with signals of cooling in some areas and continued strength in others. These findings highlight the importance of local dynamics in understanding statewide housing trends.

---

## Question 2: Explanatory  
**On average, have assessed values kept pace with actual sale prices from 2018–2023, and which property types show the largest valuation gaps?**

This question matters because assessed values play a critical role in taxation, budget planning, and public services. When assessments lag behind market values, municipalities may under-collect property taxes, creating fiscal strain. Understanding which property types are most undervalued provides insight into assessment accuracy, equity considerations, and market pressures.

To explore this question, we compared median assessed values to median actual sale prices across major property types and mapped the sales ratios (Assessed Value ÷ Sale Amount) for residential and commercial properties across Connecticut towns.

### Plot 1: Median Assessed Value by Property Type  
!![plot](./Question2_Graph1.png)

### Plot 2: Median Actual Sale Price by Property Type  
!![plot](./Question2_Graph2.png)

**Description and Results:**  
Across almost all types of real estate, assessed values fell significantly below actual sale prices. Apartments and industrial properties showed the largest gaps. For instance, apartments had a median assessed value around half their median sale price, while industrial properties were undervalued by nearly $300,000. The only outlier was public utility property, where assessed values were slightly higher than sale prices.

### Plot 3: Commercial Sales Ratio Map  
!![plot](./Question2_Graph3.png)

### Plot 4: Residential Sales Ratio Map  
!![plot](./Question2_Graph4.png)

**Description and Results:**  
Both maps reveal widespread under-assessment, with most towns shaded deep red to indicate ratios below 1.0. Residential markets, in particular, surged so quickly during COVID that assessor updates could not keep up.

**Analysis and Helpfulness of Results:**  
The clear pattern is that assessments did not keep pace with market realities. Under-assessment creates inequities between long-term residents and new buyers, affects tax fairness, and may pressure municipal budgets. These insights can help policymakers plan assessment recalibration cycles and adjust revenue expectations.

---

## Honors Question 3: Predictive  
**“Based on year-over-year sales volume trends, which Connecticut towns are likely to have increasing housing demand in the next year?”**  
*(Completed individually by Tyler Schildkraut for Honors Credit)*

Using Tableau’s forecasting model, we examined year-over-year sales counts for the 10 towns with the highest transaction volume from 2018–2023. Sales volume is an important metric because it directly reflects housing demand—more transactions indicate a more active and competitive market. We applied Tableau’s exponential smoothing forecast to project activity for 2024 and 2025.

### Forecast Visualization (2018–2025)  
!![plot](./Question3_Graph1.png)

**Description and Results:**  
The forecast suggests that Stamford, Bridgeport, and Waterbury are likely to experience increasing housing demand, as their projected lines slope upward into 2024–2025. Stamford shows a strong recovery following a 2022 decline and continues to be one of the most active markets. Bridgeport maintains high volume with steady projected growth, and Waterbury demonstrates both historical momentum and future stability.

In contrast, Hamden, New Haven, and West Hartford appear to have peaked earlier, with forecasts suggesting flat or declining demand. New Haven’s market leveled off after 2021, and West Hartford shows the clearest signs of cooling.

**Importance and Helpfulness:**  
This predictive lens helps identify which markets are likely to heat up or cool in the near future. Policymakers, developers, and local governments can use this insight to anticipate housing needs, allocate resources, and understand where competitive pressures may increase. Forecasting also highlights whether pandemic-driven demand patterns are stabilizing or continuing to shift.

---

## Tableau Packaged Workbook
The Tableau packaged workbook (**Real_Estate_CT_Analysis.twbx**) is included in this repository and contains all visualizations referenced above.

