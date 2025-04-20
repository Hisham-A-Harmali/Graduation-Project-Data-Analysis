# Analysis of Health Survey Data and Supplement Use

## Project Goal

This repository contains the R code and analysis report for a graduation research project. The primary objective was to explore factors potentially associated with dietary supplement use among survey participants, considering demographics, health indicators (BMI), and lifestyle factors. This project showcases skills in data cleaning, preparation, statistical analysis, modeling, and visualization using R.

## Data Description

* **Source:** Data was collected via a questionnaire administered to participants [Optional: Add context like 'at Jazan University' or 'in Saudi Arabia'].
* **Dataset (`data_c`):** The analysis was performed on a cleaned dataset containing responses from 321 participants.
* **Key Variables Included:** Age (Numeric), Gender (Factor), Weight (Numeric), Height (Numeric), BMI (Numeric), Original BMI Category (Factor), Education Level (Factor), Income (Numeric), Smoking Status (Factor), Supplement Use (Factor: Yes/No), plus other descriptive variables related to gym habits and supplement information sources (not all used in the final models).
* **Data Privacy:** In accordance with ethical guidelines and to protect participant privacy, the underlying dataset (`data_c`) is **not included** in this public repository.

## Methods Used

The analysis was conducted entirely in R (Version 4.4.3) using packages primarily from the `tidyverse` ecosystem and `readxl`. Key statistical methods included:

* Descriptive Statistics (Means, Medians, SD, Frequencies, Percentages)
* Chi-Square Test of Independence
* Welch Two Sample t-test
* One-Way Analysis of Variance (ANOVA)
* Pearson Correlation Test
* Binary Logistic Regression

## Key Findings Summary

* **BMI and Supplement Use:** Body Mass Index (BMI) was found to be the only statistically significant predictor of supplement use in the multivariate logistic regression model (p=0.016). Lower BMI was associated with significantly higher odds of using supplements (OR ≈ 0.94). This was supported by a bivariate t-test showing non-users had a significantly higher mean BMI than users (p=0.040).
* **Income and BMI:** A statistically significant, weak positive correlation was found between Income and BMI (r=0.24, p<0.001) after data cleaning.
* **Other Factors:** Age, Gender, Education Level, Smoking Status, and Income were *not* found to be significant predictors of supplement use in the final logistic regression model. Bivariate tests also showed no significant association between supplement use and Gender or Smoking Status. No significant difference in mean BMI was found across Education Levels (though caution is needed due to small N=1 groups for Master's/Middle School levels).
* **Sample Note:** The analysis of gym-related variables indicated all participants in the final cleaned dataset reported a reason for gym attendance.

## Repository Contents & How to View Report

* **`Analysis-of-Health-Survey-Data-and-Supplement-Use.Rmd`:** The R Markdown source file containing all code, analysis steps, and detailed interpretations.
* **`Analysis-of-Health-Survey-Data-and-Supplement-Use.html`:** The final knitted HTML report. **Please view this file directly for the full analysis, results, plots, and conclusions.**
* **`README.md`:** This file, providing a summary of the project.
* **`LICENSE`:** Contains the MIT License text.
* **`.gitignore`:** Specifies files intentionally untracked by Git (standard R template).
* **`data/` folder:** This folder is included for structure but does *not* contain the actual participant data due to privacy restrictions.

## Author & Contribution

* **Hisham A. Harmali:** Conducted all data cleaning, preparation, analysis, visualization, and reporting presented in this repository as part of a team-based graduation research project.

## License

This project's code and report files are licensed under the **MIT License** - see the `LICENSE` file for details.