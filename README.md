# :deciduous_tree:Amazon Catalog Analysis

## Objective
This project analyzes customer feedback to Amazon products to understand how the company can maximize its catalog quality.

## Data Pipeline
![From .csv, to BigQuery, to Tableau](readme_imgs/pipeline.png)
1. The dataset is extracted from [Kaggle](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset) and saved locally.
2. Missing values, improper formatting and duplicate entries are cleaned out with SQL in BigQuery.
3. The cleaned data is exported as a .csv table and fed to Tableau as a data source.
4. Data is processed into various KPIs, graphs and tables for [visualization](https://public.tableau.com/app/profile/zhongkuan.lin/viz/AmazonCatalogPerformance/AmazonProductRatingsDashboard).

## Insights
1. Catalog is performing well, with a high average rating of __4.1 stars across 1,340 different products__.
2. The catalog is dominated by products in the category of Electronics, Home Kitchen, and Computer Accessories. Most other categories only have 1 or 2 products, though __some, such as Musical Instruments, have gained popularity__.
3. Product rating count is very positively skewed. The median rating count is roughly 5000, but the upper half of products go into the tens of thousands, with the __most popular hitting over 420,000 ratings__.
4. No clear correlation between popularity and rating. Some products with less than 5,000 ratings have a score of four or more, whiile __several popular products have below average ratings__.

## Recommendations
1. __Highlight our strongest categories.__ New customers should have immediate access to the massive selection of popular items in the categories of Electronics, Home Kitchen and Computer Accessories. If expanding into new categories, a worthwhile investment would be Musical Instruments, as both items in the category have tens of thousands of ratings, well over the median of 5,000.
2. Decrease __search visibility__ of popular products with scores of less than 4 stars, and increase search visibility of less popular products with scores of 4 stars or above to take their place. This ensures customers are always exposed to the best of the catalog, facilitating sales.
3. __Investigate products with perfect 5 star ratings.__ If coming from multiple reviewers, perfect 5 star ratings are likely cases of review fraud.

## Visualization
Created a [1-page Tableau dashboard](https://public.tableau.com/app/profile/zhongkuan.lin/viz/AmazonCatalogPerformance/AmazonProductRatingsDashboard) to visualize the data.

![Amazon Catalog Performance Dashboard](readme_imgs/dashboard.png)