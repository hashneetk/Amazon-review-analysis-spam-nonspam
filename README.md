# Amazon-review-analysis-spam-nonspam
## Goal
The goal of this group project is to utilize distributed systems to analyze the Amazon Product Reviews, specifically spam vs non-spam reviews. The dataset is more than 15GB and is available on Kaggle. The dataset was stored on AWS S3 bucket. The dataset contains the ID's of the reviewer and product and the review text and score for each review. The class in the dataset represents whether a review is spam or not-spam.

## Data Pipeline
Since the dataset is huge and for easy collaboration, the data is stored on AWS S3 bucket. For easy processing of such huge dataset, the data is hosted on MongoDB Atlas with multiple sharded clusters. To improve access efficiency, indexes were set. The use of indexing allows users to efficiently perform queries by more than 20% in time. To further improve the processing time we will create clusters, configure memory allocation, and use partitions and cache.
