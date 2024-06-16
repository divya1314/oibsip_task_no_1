# Customer Segmentation Analysis

## Project Overview
This project aims to perform customer segmentation analysis using clustering techniques. By analyzing reviews, ratings, and other features of various mobile apps, we aim to identify distinct segments of customers that share similar characteristics. This analysis can help in targeted marketing, product development, and enhancing user experience.

## Dataset
The dataset used for this project includes mobile app data with the following features:
- App names
- Reviews
- Ratings
- Prices
- Sentiment polarity of reviews

The dataset file is provided in the repository:
- [user_reviews.csv](./user_reviews.csv)
- [apps.csv](./apps.csv)


## Methodology

### Data Loading and Exploration
- The dataset was loaded into a Pandas DataFrame to understand its structure and distribution of reviews, ratings, and other features.

### Data Preprocessing
- Missing values were handled, and data was cleaned.
- Numerical features were scaled for better clustering performance.
- Sentiment analysis was performed on reviews to derive sentiment polarity scores.

### Clustering
- The optimal number of clusters was determined using the Elbow Method and Silhouette Score.
- K-Means clustering algorithm was used to segment the data into different clusters.

### Cluster Profiling
- Each cluster was analyzed to understand its characteristics in terms of average sentiment polarity, average rating, total reviews, and average price.
- The top apps in each cluster were identified based on the number of reviews.

## Results
The analysis identified several customer segments. Below is a summary of the findings:

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
Based on the analysis and identified clusters, the following recommendations can be made:

1. **Targeted Marketing**: Develop marketing strategies tailored to each customer segment. For example, Cluster 2, which has high ratings and a large number of reviews, could benefit from loyalty programs and exclusive offers to maintain engagement.

2. **Product Development**: Consider the preferences of each segment when developing new features or apps. For instance, apps with high average prices in Cluster 3 suggest a market for premium features or subscription-based models.

3. **User Experience Improvements**: Enhance user experience based on feedback and sentiment analysis. Clusters with lower sentiment polarity might benefit from focused improvements in app functionality and customer support.

4. **Price Optimization**: Adjust pricing strategies based on cluster characteristics. For example, Cluster 1, with a very low average price, indicates a price-sensitive customer base.
