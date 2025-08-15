# google-play-store-analysis
Sentiment analysis and insights on Google Play Store apps and user reviews.

## Overview
This project was carried out as part of an **educational project** to explore sentiment trends and key product metrics in Google Play Store apps. The analysis combines both **app metadata** (such as categories, ratings, and installations) and **user review data** to understand sentiment trends across different app categories.

In addition, the project also analyzes key product metrics such as **ARPU**, **ARPPU**, **CAC**, **Retention Rate** and **LTV** to provide insights on how to optimize long-term profitability.

There are two main analyses:
1. **Google Play Apps Metadata Analysis**: Analysis of app metadata, including app category, rating, and install counts.
2. **Google Play Store User Reviews Sentiment Analysis**: Sentiment analysis (positive, neutral, negative) of user reviews for each app category.

## Key Insights

### 1. **ARPU vs CAC**
   - While **ARPU** fluctuates, **CAC** remains stable, indicating that **revenue per user** is growing without increasing acquisition costs.

### 2. **ARPU vs Retention Rate**
   - **Retention Rate** remains relatively constant, while **ARPU** shows more variation. This suggests that **increased revenue** is likely driven by **premium users** or better **monetization** rather than retention alone.

### 3. **ARPPU vs LTV**
   - **ARPPU** and **LTV** are highly correlated, meaning that increasing **revenue from paying users** directly boosts **long-term value**.

### 4. **Retention Rate vs LTV**
   - **Retention Rate** has less impact on **LTV** than **ARPPU**, suggesting that **retaining high-value users** is more crucial than overall retention.

### 5. **Correlation Heatmap**
   - **ARPU** and **ARPPU** show a positive correlation with **LTV**, but **Retention Rate** has weaker correlations, highlighting the importance of improving **paying user monetization**.

## Explanation

### 1. **ARPU Growth**:
   - The forecast shows a **gradual increase** in **ARPU** over the next 1-2 years, suggesting **sustained revenue growth** driven by consistent user engagement.

### 2. **Seasonality Considerations**:
   - Prophet’s ability to account for **seasonal effects** in the data helps us better understand how **ARPU** will fluctuate during different times of the year, making the forecast more accurate and realistic.

### 3. **Forecast Uncertainty**:
   - The **widening confidence intervals** illustrate the uncertainty inherent in long-term forecasting. **Prophet** provides a clear view of this uncertainty, helping decision-makers understand the potential range of future outcomes.

**Note**: *Prophet, a forecasting model developed by Facebook, was used to generate these predictions. Prophet is particularly well-suited for time series data with strong seasonal effects and long-term trends, making it ideal for predicting ARPU growth. Unlike simple models, Prophet accounts for complex seasonality, holidays, and outliers, delivering a more robust and reliable forecast.*

## Dataset Source and Time Period
- The dataset used for this analysis is from the **Google Play Store** and can be found on [Kaggle](https://www.kaggle.com/datasets/lava18/google-play-store-apps).
- The data includes app information and user reviews collected from **May 21, 2010, to August 8, 2018**, providing insights into app performance and user sentiment over that period.

## Project Structure


project-folder/
├── data/                       # Dataset files
│   ├── googleplaystore.csv
│   └── googleplaystore_user_reviews.csv
│
├── notebooks/                  # Google Colab notebooks for analysis
│   ├── google_play_apps_analysis.ipynb
│   ├── googleplaystore_user_reviews.ipynb
│   └── get_requirements.ipynb  # Script to get requirements.txt
│
├── README.md                   # Project documentation
└── requirements.txt            # Dependencies



---
