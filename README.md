# Customer Segmentation for Marketing Strategies using K-Means and Hierarchical Clustering

## Business Overview
This business initiative leverages authentic customer data to execute market segmentation, a critical element for enterprises seeking insights into customer behavior to enhance marketing efficiency. The project encompasses comprehensive data preprocessing, exploratory data analysis (EDA), feature engineering, and the application of clustering algorithms—specifically, the widely recognized k-means and hierarchical clustering techniques.

## Business Objective
1.   **Understanding Acquisition Channel Impact**<br>
Evaluate the extent to which the platform’s acquisition channels influence student learning outcomes.
3.   **Geographical Discovery**
<br>Identify geographical locations where a majority of students discover the platform, with a particular focus on social media platforms like YouTube or Facebook.

## Project Highlights
1.   **Diverse Customer Behavior Exploration**
<br>The project dives deep into the spectrum of customer behavior, unraveling distinct segments that can be strategically targeted with personalized marketing strategies.
2.   **Optimizing Marketing Approaches**
<br>The identified customer segments serve as a foundation for tailoring marketing approaches, optimizing engagement, and ultimately improving business outcomes.

## Methodology
The project employs a robust methodology, including data preprocessing, exploratory data analysis, and advanced clustering techniques. The application of k-means and hierarchical clustering ensures a comprehensive understanding of customer segments.

---

## Data Dictionary
> **Properties**

|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
| minutes_watched | float64     | Total minutes of content watched by the customer. |
| CLV             | float64   | Customer Lifetime Value, representing the total predicted value a customer will bring to the business. |
| region          | int64    | Geographical region from which the customer originates. |
| channel         | int64    | Acquisition channel through which the customer discovered the platform. |

## Dependencies
*   `pip install pandas`
*   `pip install numpy`
*   `pip install matplotlib`
*   `pip install seaborn`
*   `pip install scipy`
*   `pip install sklearn`

---

## Result Interpretation
Now that we have our customer segments, we proceed to the vital step of discussing results with the marketing team and formulating an effective marketing strategy.

### Segments Analysis
*   Twitter Devotees Segment
    *   **Observations:** 58
    *   **Recommendation:** Considering the small size of this segment, we suggest reducing spending on Twitter to a minimum. The results indicate unsatisfactory outcomes, possibly due to recent platform turmoil. We recommend exploring early adoption of a new competitor platform, such as Threads.

*   Facebook Enthusiasts Segment
    *   **Observations:** Close to 8% of all customers
    *   **Characteristics:** Although not the most significant segment, this group demonstrates high dedication to learning with an average watch time exceeding 2,700 minutes.
    *   **Recommendation:** Despite average spending in the lower half, it would be valuable to explore why this group is more motivated to study. This could be the focus of a dedicated analysis on engagement.

### Performance by Region
*   Anglo-Saxon Channel
    *   **Observations:** Largest customer segment from the USA, Canada, the UK, and Australia.
    *   **Insight:** This channel shows the best overall performance.

*   Google-YouTube Mix
    *   **Observations:** Second largest segment, with over 900 customers from the Anglo-Saxon region.
    *   **Insight:** Considerable performance, especially in the Anglo-Saxon region.

*   Rest of the World
    *   **Observations:** Over 60% of customers, with diverse geographical distribution.
    *   **Insight:** Explore how these students interact with the platform and consider tailored engagement strategies.

*   Western Europe
    *   **Observations:** Fewest customers but highest Customer Lifetime Value (CLV).
    *   **Insight:** Marketing efforts in Western Europe are insufficient; improving performance is crucial.

### Customer Lifetime Value (CLV) Analysis
*   High-Paying Clusters: Anglo-Saxon Multichannel and European Multichannel
    *   **Recommendation:** Focus on Google, YouTube, and LinkedIn as acquisition channels for these regions. Increase spending as the CLV of customers from these clusters is the highest across segments.

*   Remaining Regions and Acquisition Channels
    *   **Rest of the World:**
        *   **Successful Channel:** LinkedIn, followed by Facebook.
        *   **Recommendation:** LinkedIn is an effective platform for attracting customers from these regions due to excellent organic reach.
