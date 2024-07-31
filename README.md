# Predicting Maximum Heart Rate Achieved During Exercise

## Overview

This data science project explores the relationship between various clinical and demographic factors and the maximum heart rate (MHR) achieved during exercise. The study aims to predict MHR using machine learning techniques, utilizing data from the UCI Heart Disease Database. The project was developed in R, leveraging the powerful tools available for data analysis and machine learning.

## Motivation

Cardiovascular health is a critical component of overall well-being. Understanding the factors influencing MHR can provide insights into a person's cardiovascular fitness and potential risks. This project seeks to identify key predictors of MHR and examine how these predictors vary across different populations and locations.

## Data

The dataset used in this project is a modified version of the UCI Heart Disease Database. It includes medical information and clinical attributes from patients in four locations:

- Cleveland, Ohio, USA
- Hungary
- Swiss Confederation
- VA Long Beach, California, USA

### Key Variables

- **Age**: Age of the patient
- **Sex**: Gender of the patient
- **Resting Blood Pressure**: Patient's resting blood pressure
- **Serum Cholesterol**: Cholesterol level in mg/dl
- **Maximum Heart Rate Achieved (thalach)**: The highest heart rate achieved during exercise
- **Other clinical features**: Various other attributes, such as presence of angina, fasting blood sugar, etc.

## Objectives

1. **Primary Objective**: Can we predict the maximum heart rate achieved (`thalach`) by a patient during exercise based on their age, sex, resting blood pressure, and other clinical features?
2. **Secondary Objective**: How does the maximum heart rate of patients with identical clinical factors differ from location to location?

## Methodology

The project follows a structured approach, starting with data cleaning and exploratory data analysis (EDA) to understand the distribution and relationships between variables. The predictive modeling phase involves the use of machine learning algorithms, specifically k-Nearest Neighbors (k-NN), to predict MHR.

### Data Cleaning & EDA

- **Handling Missing Values**: Imputation of missing data points.
- **Normalization**: Scaling of numerical features.
- **Exploratory Analysis**: Visualization of data distributions and relationships.

### Model Building

- **k-Nearest Neighbors (k-NN)**: Chosen for its simplicity and effectiveness in predicting numerical outcomes. The model was trained and validated using cross-validation techniques to ensure robustness.

## Results

The k-NN model demonstrated moderate accuracy in predicting MHR, with several clinical factors significantly influencing the outcomes. However, the model's performance varied across different locations, highlighting the importance of geographical and population-specific factors.

## Discussion

The findings suggest that while clinical factors like age, sex, and resting blood pressure are important predictors of MHR, there are limitations to using a small set of predictors for such complex physiological outcomes. The study emphasizes the need for more comprehensive models that incorporate a broader range of clinical and possibly genetic factors.

## Future Work

The study opens several avenues for future research:

1. **Incorporating Additional Variables**: Including lifestyle factors, genetic information, and more detailed medical history.
2. **Exploring Non-Clinical Factors**: Investigating the impact of psychological stress or environmental conditions on MHR.
3. **Advanced Modeling Techniques**: Using more complex models, such as ensemble methods or neural networks, for better predictive accuracy.
4. **Personalized Medicine**: Examining differences in heart rate responses to exercise across diverse populations and implications for personalized healthcare.

## References

1. Lamba, D., Hsu, W. H., & Majed Alsadhan. (2021). Predictive analytics and machine learning for medical informatics: A survey of tasks and techniques. *Elsevier EBooks*, 1–35. [https://doi.org/10.1016/b978-0-12-821777-1.00023-9](https://doi.org/10.1016/b978-0-12-821777-1.00023-9)
2. Chayakrit Krittanawong et al. (2020). Machine learning prediction in cardiovascular diseases: a meta-analysis. *Scientific Reports*, 10(1). [https://doi.org/10.1038/s41598-020-72685-1](https://doi.org/10.1038/s41598-020-72685-1)
3. UCI Machine Learning Repository. (2019). [UCI.edu](https://archive.ics.uci.edu/dataset/45/heart+disease)

## Installation

To replicate the study or build upon it, clone the repository and install the necessary packages using R's package manager:

```R
# Clone the repository
git clone <repo-url>

# Install required packages
install.packages(c("tidyverse", "caret", "knitr", "rmarkdown"))
```
## Usage

The project is structured into various R scripts and Jupyter notebooks for easy navigation and understanding. To run the analysis:

1. Load the dataset.
2. Follow the data cleaning and EDA steps outlined in the notebooks.
3. Train the model using the provided scripts.
4. Evaluate the model's performance and explore further analyses.
