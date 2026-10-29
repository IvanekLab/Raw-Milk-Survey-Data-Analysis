Why Americans Choose Raw Milk: Evidence from a National Quantitative Survey
Sophia Ruser, Cristina Rojo, Katherine J Koebel, Calvin Slaughter, Ece Bulut, Renata Ivanek

We conducted a cross-sectional survey of U.S. adults (N = 1,075 eligible; N = 898 analytic sample) to identify predictors of raw milk consumption, exclusive raw milk consumption, and at-home thermal treatment of raw milk, and to characterize beliefs about the taste, nutritional value, and illness risk of raw versus pasteurized milk. We include the following R Markdown scripts for the analyses described in the study:

File	Analysis
01_data_cleaning.Rmd	Import, eligibility filtering, variable construction, and descriptive statistics. Writes the cleaned dataset used by the other scripts.
02_outcome1_raw_milk_consumption.Rmd	Model R_Any — any raw milk consumption (n = 898)
03_outcome2_exclusive_consumption.Rmd	Model R_Exclusive — exclusive raw milk consumption (n = 898)
04_outcome3_thermal_treatment.Rmd	Models T_Any (n = 163) and T_Exclusive (n = 55) — at-home thermal treatment among raw milk consumers

Run 01 first; the three outcome scripts are independent of one another and each read the cleaned dataset fresh.

Data. The scripts expect the raw Qualtrics export survey_results.csv in the working directory.

Requirements. R with tidyverse, janitor, broom, gt, scales, pROC, ResourceSelection, and car. Figures use Times New Roman.
