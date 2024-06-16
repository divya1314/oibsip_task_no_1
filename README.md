
# Sentiment Analysis and Customer Segmentation Analysis

## Project Overview
This project aims to perform comprehensive analysis using clustering techniques on mobile app data. By integrating sentiment analysis of reviews with customer segmentation based on ratings, reviews, prices, and other features, the goal is to identify distinct customer segments. These segments will help in targeted marketing, informed product development, and enhanced user experience strategies.

## Dataset
The dataset includes mobile app data sourced from two files:
- [user_reviews.csv](./user_reviews.csv)
- [apps.csv](./apps.csv)

It comprises features such as app names, reviews, ratings, prices, and sentiment polarity scores derived from reviews.

## Methodology

### Data Loading and Exploration
The dataset was initially loaded into a Pandas DataFrame for exploration and understanding of its structure and feature distributions.

### Data Preprocessing
Data cleaning steps were applied to handle missing values and ensure data quality. Numerical feature scaling was performed to optimize clustering performance. Sentiment analysis was conducted on reviews to compute sentiment polarity scores.

### Clustering
The optimal number of clusters was determined using statistical methods like the Elbow Method and Silhouette Score. The K-Means clustering algorithm was employed to segment the data into meaningful clusters.

### Cluster Profiling
Each cluster was thoroughly analyzed to uncover its unique characteristics:
- Average sentiment polarity
- Average rating
- Total reviews
- Average price

The top apps within each cluster were identified based on review counts, providing insights into popular apps among different customer segments.

## Results
The analysis revealed distinct customer segments, each characterized by specific preferences and behaviors:

### Cluster 0
- **Average Sentiment Polarity:** 0.207
- **Average Rating:** 4.22
- **Total Reviews:** 1,745,956,147
- **Average Price:** $0.53
- **Top Apps in this Cluster:**
    - Clash of Clans (148,142,685 reviews)
    - Garena Free Fire (121,336,852 reviews)
    - Candy Crush Soda Saga (102,896,145 reviews)

### Cluster 1
- **Average Sentiment Polarity:** 0.296
- **Average Rating:** 4.41
- **Total Reviews:** 2,822,539,423
- **Average Price:** $0.01
- **Top Apps in this Cluster:**
    - Crossy Road (385,010,626 reviews)
    - Cache Cleaner-DU Speed Booster (331,751,238 reviews)
    - APUS Launcher (179,286,671 reviews)

### Cluster 2
- **Average Sentiment Polarity:** 0.034
- **Average Rating:** 4.5
- **Total Reviews:** 12,308,858,343
- **Average Price:** $0.00
- **Top Apps in this Cluster:**
    - Candy Crush Saga (5,382,402,480 reviews)
    - Clash Royale (3,817,028,820 reviews)
    - 8 Ball Pool (3,109,427,043 reviews)

### Cluster 3
- **Average Sentiment Polarity:** 0.290
- **Average Rating:** 4.27
- **Total Reviews:** 322,590
- **Average Price:** $15.49
- **Top Apps in this Cluster:**
    - Golfshot Plus: Golf GPS (135,480 reviews)
    - Essential Anatomy 3 (122,640 reviews)
    - BIG Launcher (35,240 reviews)

## Recommendations
Based on the findings from sentiment analysis and customer segmentation:

1. **Targeted Marketing Strategies**: Tailor marketing campaigns to resonate with the preferences and sentiments of each identified customer segment.
   
2. **Informed Product Development**: Use insights to guide feature enhancements and new app developments that align with the needs and expectations of different segments.
   
3. **Enhanced User Experience Initiatives**: Implement improvements in user interfaces, features, and customer support based on sentiment analysis feedback.
   
4. **Optimized Pricing Strategies**: Adjust pricing models to match the willingness to pay observed across different clusters, ensuring competitive pricing and value proposition alignment.

---
