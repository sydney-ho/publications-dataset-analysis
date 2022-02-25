# Visual Analytics of Publications Data

![Alt text](https://github.com/sydney-ho/publications-dataset-analysis/blob/main/Sydney%20Ho.png)

## Background

IEEE Visualization (IEEE VIS) is the premier conference on data visualization and every year it publishes papers from top researchers in the field. In the IEEE VIS publications dataset, papers are published in different "tracks" that include various types of research. Every row in the dataset represents a paper and the columns represent the paper's different attributes. Conference and Year are two important attributes that we will be focusing on. Conference is the specific track within the publications dataset, while Year is the year in which the paper has been published. 

To understand the collection of documents, we want to answer the following questions:

  * How are papers distributed across different tracks and years?
  * What are topics that are included in this conference?
  * What are the topics in different tracks?

## Methods

1. Exploratory Data Analysis (EDA)

After data preprocessing, exploratory data analysis was used to answer preliminary questions about the publications dataset. We grouped the papers by different attributes such as 'Year' and 'Conference' to answer general questions about the data. After grouping the papers in different ways, we generated graphs to visualize these different attributes.

2. Natural Language Processing (NLP)

We used natural language processing to convert the data into a numeric representation that would allow the computer to effectively analyze and process it.

   NLP Steps Taken:

     * Removing punctuation
     * Converting text to lowercase
     * Tokenization
     * Removing stop words
     * Stemming/Lemmatization
     * Term frequency-inverse document frequency (TF-IDF) Vectorization

3. Clustering

After we obtained all the TF-IDF values of the words in the corpus, we clustered the data into four clusters using the K-Means algorithm. The clustering model grouped papers together based on words in their abstracts that had the most similarity. We constructed visualization that allowed us to view what were the most common words in each cluster.

## Results

Based on the most common keywords in each track, we can see that Vis and SciVis share a similar topic, rendering. InfoVis focuses more on visualization design, while VAST overlaps and interacts with various other fields.
