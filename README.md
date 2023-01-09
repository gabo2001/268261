# 268261
Artificial intelligence &amp; Machine Learning final project 


# Fast Fashion Recommender System

# Team members

Gabriel Stanziola 268261 “Captain
Veronica Boni 275541
Omar Lezar 273451


# Introduction

As members of the data science team at a prestigious fast fashion firm, our goal is to help increase revenues through all possible (legal) means. One key way to do this is by improving the recommendation system on our online platform. In the fast fashion industry, recommendation systems play a crucial role in driving sales and customer loyalty by suggesting relevant and personalized products to customers.

In this project, our objective is to test and compare the performance of different recommendation algorithms on our dataset in order to identify the most suitable one for our platform.

# Methods

To improve the recommendation system on our platform, we have loaded three CSV files containing customer metadata, transaction data, and article metadata using the Pandas library. We have then removed any null values in these dataframes using the fillna() method. We have then merged the three dataframes into a final dataframe using common columns customer_id and article_id.

We have also performed some basic exploratory data analysis on the final dataframe to understand the distribution of the data. This includes looking at the first and last 5 rows of the dataframe, obtaining basic statistical summaries, and plotting histograms for certain columns.

We will be testing and comparing the performance of the following recommendation algorithms:

Simple recommendation algorithm (baseline)
Collaborative filtering
Content-based recommendation
We will be implementing these algorithms using the Python programming language and the following libraries:

pandas for data manipulation and analysis
numpy for numerical computing
seaborn for data visualization
matplotlib for creating plots and charts

We will also be performing data preprocessing and feature engineering on the dataset to prepare it for use with the recommendation algorithms. This may include tasks such as handling missing values, scaling numerical features, and encoding categorical variables.

# Experimental Design

To demonstrate the effectiveness of our recommendation system, we will conduct the following experiment:

Purpose: Compare the performance of different recommendation algorithms on our dataset

Baseline: We will use a simple recommendation algorithm as a baseline and compare the performance of other algorithms to it.

Evaluation Metrics: We will use the following evaluation metrics to compare the performance of the different recommendation algorithms:

Accuracy
Precision
Recall
F1 score

We have chosen these metrics because they are commonly used in the evaluation of recommendation systems and provide a comprehensive evaluation of the performance of the algorithm.

# Results

We built and evaluated two recommendation systems: a content-based recommendation system and a collaborative recommendation system.

For the content-based recommendation system, we used the customer's purchase history and the characteristics of the products being recommended to predict the customer's preferences. We found that if the customer had a limited purchase history or their preferences were very different from the products being recommended, the recommendation system may return a low or 0 similarity score. This suggests that a content-based recommendation system may not be effective in these cases, as it relies on the information available in the customer's purchase history and the characteristics of the products being recommended.

On the other hand, the collaborative recommendation system used the co-occurrence of ratings or interactions between customers or items to predict the customer's preferences. We found that the similarity score obtained with this system could be considered normal, depending on the specific data and algorithm being used. Some algorithms, such as cosine similarity, return values between 0 and 1, where 0 indicates no similarity and 1 indicates complete similarity. Other algorithms, such as Pearson correlation coefficient, return values between -1 and 1, where -1 indicates negative correlation and 1 indicates positive correlation. A similarity score of 0.015, for example, could be considered low but still meaningful, as it may represent a small overlap in the ratings or interactions of two customers.

Overall, our results suggest that the choice of recommendation system and the specific data and algorithm being used can have a significant impact on the accuracy and effectiveness of the recommendations. It may be necessary to experiment with different approaches and evaluation metrics to determine the most appropriate recommendation system for the given task, but for what we have done, the collaborative system seems to be more reliable.

# Conclusions

Overall, our goal is to identify the most effective recommendation algorithm for our platform in order to drive sales and increase customer satisfaction. By comparing the performance of different algorithms, we can make informed decisions about which one to implement and how to further improve the recommendation system in the future. However, there may be limitations to our experiment, such as the size and representativeness of the dataset, that may affect the generalizability of our findings. There may also be other factors that influence the performance of the recommendation system, such as the quality and variety of the products on the platform and the behavior of the customers.

There are also many directions for future work that we can pursue in order to further improve the recommendation system. For example, we could explore more advanced recommendation algorithms, such as matrix factorization or deep learning-based methods, or we could incorporate additional data sources, such as customer reviews or social media activity, into the recommendation process. We could also investigate ways to optimize the recommendation system for specific segments of customers or for different types of products.

In conclusion, our work has shown that different recommendation algorithms can have significantly different performance on our dataset, and it is important to carefully evaluate and compare the performance of different algorithms in order to identify the most suitable one for our platform. There are many opportunities for further improvement and innovation in the field of fast fashion recommendation systems, and we look forward to continuing our work in this direction.
