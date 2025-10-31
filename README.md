# DSA210_PROJECT - Analyzing the Relationship Between Price and Nutrition in Diet-Labeled Products
## Motivation

Healthy eating has become a global priority, with consumers increasingly choosing products that are high in protein, low in sugar, and marketed as “fit,” “light,” or “healthy.” However, these diet-oriented products are often associated with higher prices compared to their regular counterparts.
This project aims to examine whether there is a measurable relationship between a product’s nutritional value (such as protein, sugar, fat, and calorie content) and its price.

## Data Source & Collection Process

This project will use publicly available food and nutrition datasets from reliable open-data platforms.
The primary data source will be OpenFoodFacts
, which provides detailed information about:

- Product name, brand, and category

- Nutritional values (calories, sugar, protein, fat, fiber, etc.)

- Labels and claims (e.g., “fit,” “light,” “high protein”)

- Optional price data and country of origin

To enrich the dataset, price information will also be collected from publicly accessible supermarket websites such as Migros, CarrefourSA, and A101. Products will be filtered to include those labeled as diet, fit, light, protein, or healthy to ensure the analysis focuses on diet-oriented items.

## Data Analysis Plan

1. Data Cleaning & Preparation

- Handle missing values and inconsistent units

- Standardize quantities (e.g., kcal per 100g, TL per 100g)

- Label products based on diet-related keywords

2. Exploratory Data Analysis (EDA)

- Generate summary statistics for nutritional and price variables

- Perform correlation analysis between nutrition metrics and price

- Examine whether products labeled as “fit,” “light,” or “high protein” accurately reflect healthier nutritional profiles

- Visualize price distribution across categories (boxplots, scatter plots)

3. Hypothesis Testing

- H₀: There is no significant difference in price between diet-labeled and regular products

- H₁: Diet-labeled products have significantly higher prices

Apply t-test or ANOVA depending on data structure

## Expected Findings

- Diet-labeled products are expected to have higher prices despite moderate nutritional differences.

- “Healthy” or “fit” branding may not always correspond to meaningful improvements in nutritional quality.

- Statistical testing will help verify whether the “healthy = costly” assumption holds true.

## Limitations and Future Work

- Some products may lack complete or standardized price information.

- Definitions of “healthiness” vary across product categories.

- Future studies could include cross-country comparisons or consumer perception analysis.

## Note
- AI tools such as ChatGPT were used only for writing assistance and improving clarity of this document.

