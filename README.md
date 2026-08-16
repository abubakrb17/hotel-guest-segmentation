# AI-Powered Guest Segmentation for Targeted Marketing Campaigns

## Business Problem
Hotels treat most guests the same way. This leads to wasted marketing budget and missed opportunities with high-value customers.

This project uses machine learning to segment 83,590 real hotel customers into meaningful groups and recommends specific marketing actions for each segment.

## Dataset
- Source: Real hotel customer data from a 4-star hotel in Lisbon, Portugal (2015–2018)
- Size: 83,590 customers
- Features: Demographic, behavioral, and revenue data

## Approach
1. Data cleaning and feature engineering (Total Revenue, Revenue per Night, Repeater flag)
2. Selected key behavioral and value features
3. Standardized the data
4. Applied K-Means clustering (4 segments)
5. Interpreted each segment in hotel business language

## Results – Guest Segments

| Segment | Size | Name | Avg. Total Revenue | Key Traits | Recommended Action |
|---------|------|------|--------------------|------------|--------------------|
| 3 | 1,455 | Loyal High-Value Guests | 948 | True repeaters, highest spend, longer stays | VIP treatment, loyalty offers, exclusive upgrades |
| 0 | 20,008 | High-Spending Planners | 700 | Book far in advance, high revenue | Early-bird premium packages, long-stay offers |
| 1 | 40,670 | Typical Transient Guests | 369 | Standard one-time guests | Room upgrade & breakfast upselling |
| 2 | 21,457 | Low-Engagement Guests | 11 | Almost no revenue or stays | Low marketing priority |

## Business Impact
- Identifies the small group of guests who generate the highest revenue
- Helps marketing teams stop wasting budget on low-value segments
- Supports personalized campaigns and better resource allocation

## Tech Stack
- Python, pandas, scikit-learn
- K-Means clustering
- Feature engineering for hospitality metrics
