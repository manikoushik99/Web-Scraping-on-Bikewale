🏍️ Web Scraping and Exploratory Data Analysis of Bikes from BikeWale
📘 Project Overview

This project focuses on scraping real-world bike data from BikeWale
 — one of India’s top motorcycle comparison platforms — and performing Exploratory Data Analysis (EDA) to uncover market insights on pricing, mileage, performance, and brand positioning.

The goal is to demonstrate a complete data pipeline — from web scraping to cleaning, analysis, and visualization — to derive meaningful insights about the Indian bike market.

🧩 Business Problem

Unstructured and scattered bike data makes comparison difficult.

No centralized insights for pricing, performance, or mileage analysis.

Consumers struggle to balance performance vs affordability.

Manufacturers lack clear visibility into brand positioning and competition.

Absence of analytical benchmarking hinders data-driven decisions.

🎯 Objectives

Extract and structure bike data from the BikeWale website using Python.

Clean and preprocess data for analysis and visualization.

Analyze relationships between engine capacity, power, price, and mileage.

Visualize brand-wise and segment-wise trends.

Identify top-performing brands in different categories.

Provide actionable insights for manufacturers and consumers.

🧰 Tools & Libraries Used

Python

BeautifulSoup & Requests – Web Scraping

Pandas & NumPy – Data Cleaning & Processing

Matplotlib & Seaborn – Data Visualization

Jupyter Notebook / Google Colab

🔍 Web Scraping Process

Scraped 11 pages of new bike listings from BikeWale.

Extracted key details:

Model Name

Rating & Number of Ratings

Engine Details (CC, Power, Mileage)

Price

Location

Parsed HTML using BeautifulSoup with CSS selectors.

Stored all scraped data into a Pandas DataFrame for cleaning and analysis.

🧹 Data Cleaning Steps

Removed unwanted symbols (₹, cc, kmpl) and extra spaces.

Converted numeric columns (Price, Rating, Mileage) to appropriate data types.

Split combined columns (like Engine Details) into individual fields.

Replaced missing values using NaN or average-based imputation.

Standardized brand and model names.

Removed duplicates and verified formatting consistency.

📊 Exploratory Data Analysis
🔸 Univariate Analysis

Numerical:

Ratings are concentrated around 4.5, with some high-value outliers.

Price and Engine Capacity show wide variation, reflecting diverse market segments.

Categorical:

Most bikes fall into Luxury and Budget price categories.

Medium and Low mileage bikes dominate the market.

🔸 Bivariate Analysis

Numerical vs Numerical:

Strong positive correlation between Engine Capacity and Power.

Higher Power often correlates with higher Price, though brand factors influence it.

Numerical vs Categorical:

Brands like Hero, Honda, and TVS deliver top mileage in the commuter segment.

Premium brands (KTM, Harley, BMW) focus on performance with lower mileage.

Categorical vs Categorical:

Hero, Yamaha, TVS dominate Budget & Mid-range categories.

Royal Enfield, Ducati, Kawasaki dominate Luxury segments.

🔸 Multivariate Analysis

Luxury and High-end bikes → High power, Low mileage.

Budget and Mid-range bikes → Low power, High mileage.

Clear inverse relationship between price and mileage.

💡 Key Business Questions

Which brands offer the most bike models in India?

How are engine capacity, power, and price related?

Which price segment dominates the market?

How does mileage vary by brand and price category?

Which brands offer the best mileage-to-price ratio?

How do ratings correlate with price and mileage?

🧾 Key Insights

Engine Capacity and Power show strong positive correlation.

Luxury & High-end bikes prioritize power; Budget bikes focus on efficiency.

Hero, Honda, TVS lead in fuel-efficient bikes.

KTM, Royal Enfield, BMW dominate performance-driven categories.

Price vs Mileage: As price increases, mileage decreases.

💪 Experience – Web Scraping & Data Analysis

Scraped real-world data using BeautifulSoup and Requests.

Cleaned and standardized data with Pandas and NumPy.

Conducted EDA using Matplotlib and Seaborn visualizations.

Learned end-to-end workflow:
Scraping → Cleaning → Analysis → Visualization → Insights.

⚙️ Challenges Faced

Inconsistent HTML structures across pages.

Hidden/missing fields like price and mileage.

Duplicate and inconsistent brand names.

Handling special characters (₹, cc, kmpl) in text fields.

Anti-scraping measures limiting requests.

Selecting meaningful visualizations for storytelling.

🏁 Conclusion

The project highlights the power of web scraping and data analysis in extracting real-world business insights.
It reveals that the Indian bike market is divided between performance-oriented (Luxury) and efficiency-focused (Budget) segments, with Hero, TVS, and Honda leading in affordability and mileage, while Royal Enfield and KTM dominate the premium sector.
