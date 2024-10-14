# Will a Customer Accept the Coupon?

## Context

Imagine you're driving through town and a coupon for a nearby restaurant is delivered to your phone. Would you take a detour to use the coupon immediately? Would you save it for later or ignore it? What factors influence whether you accept the coupon? Is it the type of venue—restaurant, bar, coffee shop? Does having a passenger, the weather, or the time of day make a difference? 

This project explores the factors that influence the likelihood of accepting a coupon delivered while driving.

## Project Overview

The goal of this project is to analyze customer behavior in response to driving-related coupons. We aim to explore how various factors, such as passenger type, weather, and destination, affect whether a customer accepts a coupon. Using visualizations and probability distributions, we aim to uncover patterns in customer decisions.

## Data Source

The dataset is sourced from the UCI Machine Learning repository and was collected through a survey on Amazon Mechanical Turk. The dataset provides scenarios involving driving conditions (destination, weather, passengers, etc.), and participants were asked if they would accept coupons for various establishments, such as:

- Restaurants (less than $20)
- Coffee houses
- Takeaway places
- Bars
- Restaurants ($20-$50)

### Data Summary

Each record in the dataset represents a scenario where a coupon was offered. Responses to whether the coupon was accepted are labeled as:

- `Y = 1` for accepting the coupon either right away or later
- `Y = 0` for rejecting the coupon

### Key Attributes

1. **User Attributes**:
   - Gender, age, marital status, number of children, education level, occupation, income
   - Frequency of visits to bars, coffee houses, takeaway places, and restaurants (under $20)

2. **Contextual Attributes**:
   - Destination (home, work, or no urgent destination)
   - Location and proximity to the venue
   - Weather (sunny, rainy, snowy), temperature (30F, 55F, 80F)
   - Time (10AM, 2PM, 6PM), and passengers (alone, with partner, friends, or kids)

3. **Coupon Attributes**:
   - Type of venue (restaurant, bar, coffee house, etc.)
   - Time before the coupon expires (2 hours, 1 day)

## Analysis and Methodology

### Step-by-step Approach:

1. **Data Preprocessing**:
   - Handling missing values by either dropping or imputing data.
   - Cleaning and transforming the dataset for analysis.

2. **Exploratory Data Analysis**:
   - Visualizations of acceptance rates by different coupon types and user characteristics.
   - Bar plots and histograms for factors like coupon type, temperature, and acceptance rates.

3. **Specific Investigations**:
   - Analyzing acceptance rates for bar coupons, comparing users based on bar visitation frequency, age, and presence of passengers.
   - Comparing acceptance rates for users going to bars more than once a month with different income levels or marital statuses.
   
4. **Independent Investigation**:
   - Examining characteristics of users accepting coupons for restaurants under $20, focusing on factors like income and age.

## Key Findings

### General Coupon Acceptance Rates
- The overall acceptance rate for coupons varies by type and context, with restaurants and coffee houses generally having higher acceptance rates than bars.

### Bar Coupons
- People who visit bars more frequently (more than 3 times per month) are more likely to accept bar coupons, especially if they are under 30 or have a partner as a passenger.

### Restaurants Under $20
- Users with an income below $50K and younger than 25 tend to accept restaurant coupons for less expensive meals more frequently.

## Conclusion

This project provides insight into how various factors influence the acceptance of driving-related coupons. The findings could help businesses tailor their marketing strategies by targeting the right customers at the right time and place.

## Tools and Libraries

- Python (Pandas, Matplotlib, Seaborn)
- Jupyter Notebook
- Plotly for interactive visualizations

## License

This project is licensed under the MIT License.