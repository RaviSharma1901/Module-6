# Myntra Online Retail Customer Segmentation

## Project Overview

**Project Name:** Unsupervised ML - Myntra Online Retail Customer Segmentation  
**Project Type:** EDA & Unsupervised Learning - RFM and K-Mean Clustering  
**Contribution:** Individual  
**Author:** Ravi Sharma

This project focuses on leveraging customer transaction data from Myntra, a leading Indian fashion e-commerce platform, to segment the customer base using RFM analysis and K-Means clustering. The analysis includes records from Myntra Gifts Ltd., its UK-based subsidiary, to understand purchasing behavior across different markets and implement targeted marketing strategies.

## Problem Statement

Myntra faces challenges in marketing to its heterogeneous customer base. This project aims to utilize historical retail transaction data to uncover actionable customer segments using unsupervised machine learning techniques. By applying RFM (Recency, Frequency, Monetary) analysis and K-Means clustering, we intend to:

- Analyze customer behavior patterns deeply
- Segment customers effectively for targeted marketing
- Drive personalized marketing strategies
- Improve customer retention rates
- Understand diverse purchasing patterns across different markets

## Dataset Features

| Feature | Description |
|---------|-------------|
| **InvoiceNo** | Unique transaction identifier for tracking purchase history |
| **StockCode** | Product-specific identification for analyzing purchasing patterns |
| **Description** | Product names providing context to customer preferences |
| **CustomerID** | Unique customer identifier for building customer-level insights |
| **Country** | Geographic data for exploring location-based purchasing trends |
| **Quantity** | Number of units bought per product in each transaction |
| **UnitPrice** | Price per unit of each product for monetary calculations |
| **InvoiceDate** | Transaction timestamp for determining recency in RFM analysis |

## Methodology

### RFM Analysis
The foundation of customer segmentation based on three key metrics:

- **Recency (R):** How recently a customer made a purchase
- **Frequency (F):** How often a customer makes purchases  
- **Monetary (M):** Total spending amount of a customer

This analysis provides a comprehensive picture of customer value and engagement levels.

### K-Means Clustering
Using RFM scores as features, K-Means clustering algorithm groups customers based on their behavior patterns into distinct segments, enabling customized engagement strategies.

## Results & Customer Segments

### Optimal Clustering: K=4

#### Cluster 0: Inactive Customers
- **Recency:** 190 days (Haven't purchased recently)
- **Frequency:** 1.37 purchases (Rarely shop)
- **Monetary:** $351.75 (Low spending)
- **Strategy:** Reactivation campaigns, special discounts, reminders

#### Cluster 1: Loyal Customers
- **Recency:** 59 days (Occasional purchases)
- **Frequency:** 4.42 purchases (Moderate engagement)
- **Monetary:** $1,783.12 (High value customers)
- **Strategy:** Personalized recommendations, repeat purchase incentives

#### Cluster 2: VIP Customers
- **Recency:** 10 days (Recently active)
- **Frequency:** 13.98 purchases (Frequent shoppers)
- **Monetary:** $7,484.82 (Highest value segment)
- **Strategy:** VIP perks, loyalty programs, early access to collections

#### Cluster 3: Occasional Buyers 
- **Recency:** 23 days (Recent but inconsistent)
- **Frequency:** 1.87 purchases (Occasional buyers)
- **Monetary:** $453.33 (Medium spending)
- **Strategy:** Introductory offers, bundle deals, personalized nudges

## Key Outcomes

- **Data-driven Segmentation:** Enables Myntra to personalize promotions effectively
- **Optimal Clustering:** K=4 clusters provide meaningful customer segmentation
- **Customer Personas:** Clear definition of VIP, Loyal, Occasional, and Inactive customers
- **Actionable Strategies:** Specific marketing approaches for each customer segment

## Technologies Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Scikit-learn** - Machine learning algorithms (K-Means)
- **Matplotlib/Seaborn** - Data visualization
- **Jupyter Notebook** - Development environment

## Getting Started

### Prerequisites

    pip install -r requirements.txt

### Running the Analysis
1. Clone the repository
    
       git clone https://github.com/RaviSharma1901/Module-6
       cd "Module-6/End_Course_Capstone_Project_ML"

3. Open the Jupyter notebook

       jupyter notebook Mid_Course_Assessment_ML_Case_Study_Ravi_Sahrma.ipynb
   
5. Run all cells sequentially
6. View results and visualizations

## Business Impact

This customer segmentation analysis enables Myntra to:
- **Increase Revenue:** Target high-value VIP customers with premium offerings
- **Improve Retention:** Re-engage inactive customers with personalized campaigns
- **Optimize Marketing Spend:** Focus resources on the most responsive customer segments
- **Enhance Customer Experience:** Provide personalized recommendations based on segment behavior

## Links

* **Email**: [ravisharma1901@gmail.com](mailto:ravisharma1901@gmail.com)
* [LinkedIn](https://www.linkedin.com/in/ravi-sharma-ab8ba17a/)  
* [GitHub Profile](https://github.com/RaviSharma1901)

