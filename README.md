# PROG8431_Group2_Predicting_and_Managing_Soil_Acidification
## Group Members
### Aiswarya Thekkuveettil Thazhath - 8993970
### Albright Maduka Ifechukwude - 9053136
### Abdullahi Abdirizak Mohamed   -   9082466

### 1. Project Overview

This project analyzes how nitrogen fertilizer usage affects soil acidity (pH) across different agricultural regions in Canada.
Long-term use of ammonium-based nitrogen fertilizers is known to acidify soils, which reduces nutrient availability, increases toxic metals, and decreases crop yield.

The goal is to build a data-driven system that predicts when and where fertilizer use will significantly lower soil pH and provides recommendations to maintain optimal soil health and sustainable farming.

### 2. Problem Statement

Long-term use of ammonium-based nitrogen fertilizers is acidifying soils across Canada.
Falling soil pH reduces nutrient availability, increases toxic metals, and lowers crop performance — forcing farmers to apply lime and incur extra costs.

Objective:
To analyze the relationship between nitrogen fertilizer levels and soil pH, and to determine whether higher nitrogen use significantly decreases pH.

### 3. Dataset Description

We used the dataset Crop_recommendationV2.csv, which contains about 2,200 soil samples collected from various regions.
Each record includes the following features:

Feature	Description
N	Nitrogen content in soil (mg/kg)
P	Phosphorus content in soil (mg/kg)
K	Potassium content in soil (mg/kg)
temperature	Temperature in °C
humidity	Relative humidity (%)
rainfall	Rainfall in mm
ph	Soil pH level
label	Recommended crop type

Focus Columns for This Study:

N (Nitrogen)

pH (Soil Acidity)

### 4. Hypotheses

H₀ (Null Hypothesis):
Nitrogen fertilizer use has no significant effect on soil pH.

H₁ (Alternative Hypothesis):
Higher nitrogen fertilizer use lowers soil pH — making the soil more acidic.

### 5. Methodology
Data Analysis Tools Used

Language: Python

Libraries: pandas, numpy, scipy, seaborn, matplotlib

Steps Performed

- Loaded the dataset and checked for missing values

- Focused on the N and pH columns

- Calculated descriptive statistics (mean, median, mode, variance, standard - deviation)

- Created distribution plots for pH and Nitrogen

- Performed a Pearson correlation test to check the relationship between Nitrogen and pH

### 6. Key Results
Metric	Soil pH	Nitrogen (N)
Mean	6.47	50.55
Median	6.42	37.00
Mode	3.50	22.00
Variance	0.59	1362.89
Standard Deviation	0.77	36.92
Observations

- The mean pH indicates slightly acidic soil.

- Nitrogen levels vary widely, while pH remains relatively stable.

- The pH histogram forms a smooth bell-shaped curve, showing most soils are near-neutral.

- The Nitrogen histogram shows uneven distribution — fertilizer levels differ across farms.

### Statistical Test

### Correlation Coefficient (r): Negative

p-value: < 0.05

### Conclusion

Since the p-value is below 0.05, we reject the null hypothesis (H₀) and accept the alternative hypothesis (H₁).
This confirms that higher nitrogen fertilizer use significantly reduces soil pH, supporting the evidence of fertilizer-induced acidification.
