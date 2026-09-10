# Hotel Guest Segmentation

Customer segmentation project using Python and K-Means clustering to identify distinct hotel guest groups and translate behavioral patterns into actionable business strategies.

## Project Overview

This project analyzes a hotel customer dataset containing 83,590 guest records and 31 variables.

The objective was to segment customers into meaningful groups based on booking behavior, revenue contribution, stay activity, and recency so that hotel managers can design more targeted retention, loyalty, acquisition, and promotional strategies.

The analysis combines:

- data cleaning
- feature engineering
- exploratory analysis
- feature scaling
- K-Means clustering
- Elbow Method
- Silhouette Score
- cluster profiling
- business interpretation

## Business Problem

Hotels serve customers with very different booking habits, spending levels, stay frequency, and planning behavior.

Treating every guest the same can reduce marketing efficiency and weaken retention strategies.

This project aims to answer:

- Which customer groups generate the most value?
- Which guests are most likely to behave like loyal customers?
- Which customers book far in advance?
- Which guests show very limited historical activity?
- How should hotel management approach each segment differently?

## Dataset

The dataset contains approximately **83,590 customer records** and **31 variables**.

Key variables used in the analysis include:

- Age
- AverageLeadTime
- LodgingRevenue
- OtherRevenue
- RoomNights
- BookingsCheckedIn
- DaysSinceLastStay

Additional customer and booking characteristics were available in the original dataset.

## Data Preparation

The dataset was cleaned before clustering.

Main preparation steps included:

1. loading the Excel dataset with pandas
2. checking data types and missing values
3. handling missing Age values
4. correcting invalid or negative values where appropriate
5. creating derived business features
6. selecting relevant clustering variables
7. standardizing numerical features using `StandardScaler`

### Feature Engineering

Three additional variables were created:

**TotalRevenue**

Combined lodging and other revenue:

```python
TotalRevenue = LodgingRevenue + OtherRevenue
