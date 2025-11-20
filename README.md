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
We chose the data model title Real Estate Sales 2001-2023 GL. Specifically, our data was collected from the state of Connecticut and we have narrowed our focus more specifically on the past decade or so of housing prices. It included exactly 1,141,722 rows of values along with 14 columns in total so we really wanted to make sure we narrowed down our filters and the scope of our analysis. The reason we chose this data set was because we were curious about trends in recent years as the housing market is always a great indicator of market health. Additionally, our data set is rich in values that people can understand. Some of the most relevant data we were able to get plenty of information on were the following: Serial Number, List Year, Town, Address, Assessed Value, Sale Amount, Sales Ratio, Property Type, and Residential Type. Other data included in the database included Date Recorded, Non Use Code, Assessor Remarks, OPM Remarks, and Location. However, we made the decision to not include analysis of these values because they were redundant, not extremely intuitive, and we found we could provide better insights using other data points specified in the model. Serial Number (whole number data type) specifies the unique label placed on each individual house in the state of Connecticut. List Year (whole number data type) specifies the year the house was listed on the market and Data Recorded (date data type) is the specific date the property was registered under a specific mortgage/deed. Town (string data type) and Address (string data type) included information about where the house was located. Assessed Value (decimal number data type) and Sales Amount (decimal number data type) allowed us to examine the difference between what the value of the house was assessed to be by appraisers versus the amount the house actually sold for on the market. The Sales Ratio (decimal number data type) provides a specific ratio that details the discrepancies between Assessed Value and Sales Amount. For example, a ratio below 1.0 would be indicative of a property being under-assessed versus a ratio above 1.00 indicating the property is being over-assessed. Property Type (string data type) indicates the specific property type (Residential, Commercial, Vacant Land, etc.). Residential Type (string data type) specifies the specific residential property type given that the property is considered Residential (Single Family, Two Family, Condo, etc.). Non-Use Code (string data type) specifies information regarding a property if it was regarded as not conforming property contractual obligations. Assessor Remarks (string data type) specifies official remarks given by a property assessor for tax purposes, and OPM Remarks (string data type) includes information regarding if a property was financed by an outside source other than the purchaser’s own funds. Lastly, Location (string data type) provides the exact GPS coordinates of a specific property.


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

