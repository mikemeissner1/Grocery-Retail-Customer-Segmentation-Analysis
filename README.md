# Customer Segmentation for Strategic Marketing Analysis

## Table of Contents
- [Executive Summary](#executive-summary)
- [Project Overview](#project-overview)
- [Team Members](#team-members)
- [Data Description](#data-description)
- [EDA](#exploratory-data-analysis)
- [Methodology](#methodology)
- [Analysis](#analysis)
- [Key Findings](#key-findings)
- [Strategic Recommendations](#strategic-recommendations)
- [Business Implications](#business-implications)

## Executive Summary

In this comprehensive analysis of a grocery firm's customer database, our team identified four distinct consumer segments using K-Means clustering. These segments - "The Affluent Connoisseurs", "Budget-Focused Digital-Savvy Young Parents", "Upper Mid-Level Affluents", and "The Economical Engagers" - provide a foundation for tailored marketing strategies. Our recommendations range from curated wine selections to bulk economy buys, designed to resonate with each segment's unique characteristics and preferences.

## Project Overview

### Objective
To develop a data-driven customer segmentation model and create targeted marketing strategies for a grocery firm, addressing the current gap in customer understanding and resource allocation.

### Stakeholder
Chief Marketing Officer (CMO)

### Goals
1. Implement K-means clustering to identify distinct customer segments
2. Utilize linear regression to develop segment-specific marketing plans
3. Enhance campaign effectiveness and align with specific customer needs

## Team Members
- Adela Cho
- Mike Meissner
- Joey Gaule
- Joseph Strickland

## Data Description

The dataset, provided by Prof. Omar Rome Hernandez from the Haas School of Business at UC Berkeley, comprises aggregated customer purchase information from the grocery firm's database.

### Key Features:
- Demographic data (birth year, education, marital status, income)
- Household composition (children, teenagers)
- Purchase history across product categories
- Response to marketing campaigns
- Customer engagement metrics (web visits, complaints)

## Exploratory Data Analysis

<p align="center">
  <img width="354" alt="Screenshot 2024-10-14 at 5 03 02 PM" src="https://github.com/user-attachments/assets/7f6b04e1-9f5a-4ef2-933f-eaf707958c39">
</p>
<p align="center">
  <em>Analysis of Categorical Features. Total Levels  in “Marital Status” and “Education”
</em>
</p>


<p align="center">
  <img width="347" alt="Screenshot 2024-10-14 at 5 05 37 PM" src="https://github.com/user-attachments/assets/d02b9c5e-b96a-4dd3-8393-aeabd3a00048">
</p>
<p align="center">
  <em>Counts for Featured Variables </em>
</p>

## Methodology

1. **Data Preprocessing**
   - Removal of NA values, outliers, and duplicates
   - Categorical feature encoding
   - Data scaling for model consistency

2. **Feature Engineering**
   - Creation of derived features to enhance model performance

3. **Model Selection and Implementation**
   - Unsupervised Learning: K-means clustering for customer segmentation
   - Supervised Learning: Multiple linear regression for marketing plan development

4. **Model Validation**
   - Hold-out sampling technique for unbiased evaluation

## Analysis

### K-Means Clustering
- Optimal cluster number (4) determined via Elbow method and Scree plot analysis
- Cluster sizes also made the most sense at k=4 clusters 
- Applied Kmeans Clustering to dataset and then used centroids to determine customer segments

<p align="center">
  <img width="860" alt="Screenshot 2024-10-14 at 5 22 46 PM" src="https://github.com/user-attachments/assets/5808f5fc-deac-4dad-bfab-3d0edc07d2b9">
</p>
<p align="center">
  <em>Elbow and Scree Plots to Determine Optimal Number of Clusters
</em>
</p>

### Linear Regression
To complement our clustering analysis, we employed multiple linear regression:

- Ran separate regressions for each of the four clusters
- Created a new "quantity" variable as the target or predictor, which was made up of the total number of web purchases made by a customer
- Focused on identifying products that drive more purchases in each cluster
- Analyzed coefficients to understand cluster-specific purchase behaviors

This approach allowed us to quantify product preferences within each segment and provide data-driven insights for tailored marketing strategies.

<p align="center">
  <img width="410" alt="Screenshot 2024-10-14 at 5 40 14 PM" src="https://github.com/user-attachments/assets/05bfbc08-fc24-4da2-9f0f-0d6f53d0a4f2">
</p>
<p align="center">
  <em>Output of Regression
</em>
</p>

## Key Findings

Four distinct customer segments were identified:

1. **The Affluent Connoisseurs**
   - High-income demographic with preference for premium products
   - Significant spending on wines, fruits, and meats
   - Low presence of children/teenagers in household

2. **Budget-Focused Digital-Savvy Young Parents**
   - Lower income bracket with young families
   - Price-sensitive across all product categories
   - High engagement with digital platforms

3. **Upper Mid-Level Affluents**
   - Moderate income with balanced spending patterns
   - Active online shoppers
   - Diverse family structures

4. **The Economical Engagers**
   - Lower-middle income with larger families
   - Focus on necessity purchases
   - Engaged across multiple purchase channels

## Strategic Recommendations

Tailored marketing strategies for each segment:

1. **The Affluent Connoisseurs**
   - Exclusive wine subscriptions
   - Premium gourmet hampers
   - Luxury sweet and gold gift sets

2. **Budget-Focused Digital-Savvy Young Parents**
   - Family-oriented value packs
   - Educational product bundles
   - Targeted digital deal alerts

3. **Upper Mid-Level Affluents**
   - Virtual wine tasting experiences
   - Balanced, convenient meal kits
   - Eco-friendly product highlights

4. **The Economical Engagers**
   - Bulk purchase incentives
   - Practical loyalty rewards program
   - Budget-friendly cooking workshops

## Business Implications

- Enhanced precision in marketing efforts through segment-specific strategies
- Potential for improved customer satisfaction and loyalty across all segments
- Data-driven insights to guide future product development and inventory management
- Optimized resource allocation for marketing initiatives

This analysis provides a robust framework for the CMO to implement data-driven, targeted marketing campaigns, potentially leading to increased customer engagement and sales performance across diverse customer segments.
