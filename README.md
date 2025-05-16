# Zomato Customer Behavior and Restaurant Ratings Analysis

## Overview
This project explores a restaurant dataset from Zomato to uncover insights into customer behavior, restaurant ratings, and cost trends. Through detailed data cleaning and exploratory data analysis (EDA), we investigate how factors like location, table booking, restaurant type, and service offerings influence customer engagement and satisfaction.

## Objectives
- Clean and preprocess raw Zomato restaurant data
- Transform and standardize rating and cost columns
- Handle missing values and outliers effectively
- Answer key business-focused research questions using visual and statistical analysis

## Dataset
- Source: Zomato Kaggle Dataset (downloaded via `kagglehub`)
- Includes features like:
  - Rate, Votes, Online Order, Table Booking
  - Restaurant Type, Listed Location, Average Cost
  - City, Cuisine, Service Type

## Key Steps

### 1. Data Cleaning
- Dropped high-NA and irrelevant columns (`dish_liked`, `menu_item`, `reviews_list`, etc.)
- Converted string-based cost and rating columns to `float`
- Replaced `NEW` and `-` ratings with NaN and filled with the mean
- Final dataset contains no missing values

### 2. Outlier Detection and Treatment
- Used **IQR method** to detect and remove outliers in:
  - `rate`
  - `votes`
  - `approx_cost(for two people)`
- Visualized distributions before and after filtering

### 3. Research Questions Addressed
- What factors influence customer ratings?
- Do online orders or table bookings affect votes and ratings?
- Which restaurant types and cities score the highest ratings?
- How do cost and popularity vary by location and service type?

### 4. Insights Extracted
- Votes have the strongest correlation with ratings
- Restaurants with online orders or table booking receive more votes
- Formal dining types tend to have higher costs
- Certain areas show higher customer engagement and ratings

## Technologies Used
- Python
- pandas, numpy
- seaborn, matplotlib
- kagglehub

## Results
- Cleaned and analyzed the Zomato dataset using EDA
- Visualized trends in cost, votes, and ratings
- Answered 8 business questions that can guide restaurant marketing and operations

