# :deciduous_tree:Amazon Catalog Analysis

## Objective
This project analyzes customer feedback to Amazon products to understand how the company can maximize its catalog quality.

## Data Pipeline
![From .csv, to BigQuery, to Tableau](readme_imgs/pipeline.png)
1. The dataset is extracted from [Kaggle](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset) and saved locally.
2. Missing values, improper formatting and duplicate entries are cleaned out with SQL in BigQuery.
3. The cleaned data is exported as a .csv table and fed to Tableau as a data source.
4. Data is processed into various KPIs, graphs and tables for [visualization](https://public.tableau.com/app/profile/zhongkuan.lin/viz/AmazonCatalogPerformance/AmazonProductRatingsDashboard).


## Recommendations

## Visualization