# Netflix Movies & TV shows Clustering
## Project Description
The goal of this project is to analyze the Netflix catalog of movies and TV shows, which was sourced from the third-party search engine Flixable, and group them into relevant clusters. This will aid in enhancing the user experience and prevent subscriber churn for the world's largest online streaming service provider, Netflix, which currently boasts over 220 million subscribers as of 2022-Q2. The dataset, which includes movies and TV shows as of 2019, will be analyzed to uncover new insights and trends in the rapidly growing world of streaming entertainment.
## Problem Statement
Netflix is a streaming service that offers a wide variety of television shows and movies for viewers to watch at their convenience. With a monthly subscription, users have access to a vast library of content, including original series and films produced by Netflix. The platform also allows users to create multiple profiles, making it easy for family members or roommates to have their own personalized viewing experience. Additionally, Netflix allows users to download content to watch offline, making it a great option for those who travel frequently or have limited internet access. Overall, Netflix is a convenient and cost-effective way to access a wide variety of entertainment.

As of 2022-Q2, more than 220 million people had signed up for Netflix's online streaming service, making it the largest OTT provider worldwide. To improve the user experience and prevent subscriber churn, they must efficiently cluster the shows hosted on their platform.

By creating clusters, we will be able to comprehend the shows that are alike and different from one another. These clusters can be used to provide customers with individualized show recommendations based on their preferences.

This project aims to classify and group Netflix shows into specific clusters in such a way that shows in the same cluster are similar to one another and shows in different clusters are different.

## Analysis
The goal of this project is to analyze the Netflix catalog of movies and TV shows, which was sourced from the third-party search engine Flixable, and group them into relevant clusters. This will aid in enhancing the user experience and prevent subscriber churn for the world's largest online streaming service provider, Netflix, which currently boasts over 220 million subscribers as of 2022-Q2. The dataset, which includes movies and TV shows as of 2019, will be analyzed to uncover new insights and trends in the rapidly growing world of streaming entertainment.   

In our project we first did bit of data wrangling to understand our dataset there are approximatly **7787 records and 12 attributes** in our dataset. We then did **Exploratory Data Analysis** to understand the nature of each of the attributes in our dataset, After that we handled our **missing values** and **outliers** in the dataset, and then we did text preprocessing.   

 In **text preprocessing** we have **combined the attributes cast, country, genre, director, rating, and description**  to create different clusters. **The TFIDF vectorizer** was used to tokenize, preprocess, and vectorize the values in these attributes. After TFIDF we have to reduce dimension as there were lot of features, problem of dimensionality was dealt with through the use of **Principal Component Analysis (PCA)**. USing PCA we have reduced 10,000 features to 3000 features which explains more than **80% of our variance**.   

We have used **Kmeans** and **Agglomerative clustering** techniques to form relevent clusters we have used techniques like the **elbow method**, **silhouette score** to determine optimal number of clusters in Kmeans, while we have used **dendrogram** to determine optimal number of clusters in agglomerative clustering, we have got **6 clusters for Kmeans** and **9 clusters for agglomerative clustering.**   

After doing clustering analysis, we have developed a **Content based recommender system** which will recommend top 10 similar movies or show based to the user's current movie choice. We have used **cosine similarity** to compute similarity score between two items.
