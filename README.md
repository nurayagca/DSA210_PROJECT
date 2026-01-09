# DSA210 Project  
## Airbnb Listings and Annual Revenue Analysis

---

## Motivation
Airbnb has become a widely used platform for short-term rentals, where hosts generate income based on various listing characteristics. However, not all listings perform equally, and factors such as property type, host status, and user ratings may influence revenue outcomes.

The motivation of this project is to explore which Airbnb listing features are associated with higher annual revenue and to examine how these relationships vary across different cities.

---

## Data Source
The dataset used in this project is a publicly available Airbnb listings dataset obtained from Kaggle:

👉 https://www.kaggle.com/datasets/airbnb/airbnb-listings-data

The dataset includes information on:
- Listing details (property type, room type, amenities)
- Host attributes (Superhost status)
- Pricing and performance metrics (average daily rate, occupancy, annual revenue)
- User ratings and review counts
- Location-related variables

For the analysis, data from the following cities were combined:
Toronto, London, New York City, San Francisco, Miami, Tokyo, Sydney, Los Angeles, and Dubai.

All data used in this project is public and does not include personal or sensitive information.

---

## Data Preparation and Feature Engineering
Several preprocessing steps were applied to prepare the data for analysis:
- Column names were standardized and data types were corrected.
- Missing or invalid revenue values were removed.
- Annual revenue was log-transformed to reduce skewness.
- Additional features were created to enrich the dataset, including:
  - Median annual revenue at the city level
  - Revenue per booking
  - Revenue per available day
  - Revenue relative to the city median

These steps helped improve comparability across cities and supported later analysis.

---

## Exploratory Data Analysis
Exploratory analysis was conducted to better understand the data:
- Revenue distributions were examined.
- City-level comparisons were made using median annual revenue.
- Visualizations highlighted differences across cities and listing types.

---

## Hypothesis Testing
The following hypotheses were tested:

- **H1:** Superhost listings generate higher annual revenue than non-Superhost listings.  
- **H2:** Entire home listings generate higher annual revenue than private room listings.  
- **H3:** There is a relationship between user ratings and annual revenue.

Mann–Whitney U tests and Spearman correlation analysis were used due to non-normal revenue distributions.

---

## Machine Learning Approach
A machine learning model was used to predict annual Airbnb revenue:
- The dataset was split into training and test sets.
- A preprocessing pipeline handled missing values and categorical variables.
- A Linear Regression model was trained using log-transformed annual revenue.
- Model performance was evaluated using RMSE and R².

The model showed strong performance, indicating that listing characteristics explain a large portion of revenue variation.

---

## Key Findings
- Superhost listings tend to earn higher annual revenue.
- Entire home listings generate more revenue than private room listings.
- User ratings are statistically related to revenue, although the effect size is small.
- Revenue levels vary substantially across cities.

---

## Limitations and Future Work
- Only a linear regression model was included due to computational constraints.
- More complex models could be explored with additional resources.
- External data sources could further enrich the analysis.
- Future work could examine seasonal or time-based patterns in revenue.

---

## Note on AI Usage
AI tools such as ChatGPT were used for writing assistance and improving clarity.  
All analysis and implementation decisions were made by the author.
