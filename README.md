### Netflix Movies and TV Shows Clustering
Project Overview
This project focuses on clustering Netflix movies and TV shows based on their descriptions using unsupervised machine learning techniques. The goal is to group similar content together to enhance recommendation systems and content organization on the platform.

Dataset
The dataset contains information about Netflix movies and TV shows as of 2019, collected from Flixable, a third-party Netflix search engine. It includes features such as:

show_id: Unique ID for each show

type: Whether the content is a movie or TV show

title: Title of the show

director: Director(s) of the content

cast: Main cast members

country: Country of production

date_added: When the content was added to Netflix

release_year: Original release year

rating: Content rating

duration: Length of the content

listed_in: Genre(s)

description: Text description of the content

Key Features
Exploratory Data Analysis (EDA): Visualized distributions and trends in Netflix content

Text Preprocessing: Cleaned and transformed description text for clustering

Clustering Models: Implemented and compared three clustering algorithms:

K-Means Clustering

Hierarchical (Agglomerative) Clustering

DBSCAN Clustering

Model Evaluation: Used silhouette scores to evaluate clustering performance

Technical Approach
Data Preprocessing:

Handled missing values

Converted date features to datetime objects

Processed text data (lowercasing, removing punctuation, stopwords, etc.)

Applied TF-IDF vectorization to text descriptions

Clustering:

Determined optimal number of clusters using elbow method and silhouette scores

Implemented and compared multiple clustering algorithms

Visualized clusters using PCA for dimensionality reduction

Evaluation:

Compared models using silhouette scores

Selected best performing model for final implementation

Results
K-Means performed best with 12 clusters (silhouette score: 0.08)

Hierarchical Clustering showed good performance with 9 clusters

DBSCAN didn't perform as well on this dataset

Business Impact
The clustering results can help Netflix:

Improve content recommendation systems

Better organize their content library

Identify content gaps in their catalog

Enhance user experience through more accurate content grouping

Requirements
Python 3.x

Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, nltk, wordcloud

How to Run
Install required libraries: pip install -r requirements.txt

Run the Jupyter notebook: jupyter notebook netflix_clustering.ipynb

Future Work
Incorporate additional features for clustering (genre, cast, etc.)

Experiment with other clustering algorithms

Develop a content recommendation system based on the clusters

Implement a web application for interactive exploration of the clusters
