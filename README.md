### Description

This workshop introduces topic modeling with unsupervised machine learning in Python. Through a series of Jupyter notebooks, participants explore how K-means clustering and Latent Dirichlet Allocation (LDA) can identify patterns and topics in collections of text.

The workshop begins with deliberately simplified examples that make the behavior of the algorithms easier to inspect. Participants can examine how text is represented numerically, how words contribute to clusters and topics, and how documents relate to the resulting models.

The methods are then applied to transcripts from a YouTube lecture series, "On Power and Politics in Today's World." These related lectures provide a collection of text for investigating topics across documents. Additional examples explore simulated data, visualization, and document similarity.

### Objectives

Through a series of examples and exercises, participants will learn to:

1. Retrieve transcripts from YouTube videos, store them in pandas DataFrames, and query their text and timestamps.

2. Prepare text for analysis through cleaning, stopword removal, lemmatization, and grouping transcript segments into larger documents.

3. Represent text numerically using word counts and term frequency–inverse document frequency (TF-IDF).

4. Use K-means clustering to group documents and inspect the terms associated with each cluster.

5. Use LDA to explore topics as distributions over words and documents as mixtures of topics.

6. Investigate model behavior using simplified and simulated data, then apply the methods to lecture transcripts.

7. Explore additional approaches to interpreting and comparing text, including word clouds, interactive topic visualizations, and sentence embeddings.

### Prerequisites

This workshop is intended for participants with some experience using Python, pandas, and SQL, along with introductory machine learning experience using scikit-learn. Participants should be comfortable working with lists and dictionaries, using loops and functions, manipulating DataFrames, and fitting and applying a machine learning model.

No previous experience with topic modeling is expected. The examples introduce text preparation and representation in the context of the analysis.

## Workbooks

This workshop introduces topic modeling through a series of Python-based Jupyter notebooks. Further explanatory text is available within the workbooks.

The workbooks cover data collection and preparation, simplified modeling examples, and applications to lecture transcripts. Additional examples explore simulated data, document similarity, and visualization.

### [Extract-Query-Transcripts.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Extract-Query-Transcripts.ipynb)

Retrieve transcripts from a series of YouTube videos, inspect the returned data, and combine the transcripts into a pandas DataFrame. Use SQL to query text and timestamps, locate references to a subject, and export the results to a CSV file.

### [Youtube-API-Example.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Youtube-API-Example.ipynb)

A short example of retrieving a transcript for a single YouTube video and inspecting its text.

### [Prep-Data.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Prep-Data.ipynb)

Prepare lecture transcripts for text analysis. Clean the text, remove stopwords, apply lemmatization, and use SQL to combine consecutive transcript segments into larger documents. Export the prepared data for use in the modeling workbooks.

### [Simple-Kmeans.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Simple-Kmeans.ipynb)

Use short passages about economics and literature to illustrate K-means clustering. Represent the documents using TF-IDF, inspect the terms associated with each cluster, and assign a new passage to a cluster.

### [Simple-LDA.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Simple-LDA.ipynb)

Use the same economics and literature passages to introduce LDA with scikit-learn. Inspect document-topic weights and topic-word weights, and examine the topic mixture assigned to a new passage.

### [Topic-Modeling-Kmeans.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Topic-Modeling-Kmeans.ipynb)

Apply K-means clustering to the prepared lecture transcripts. Inspect the highest-weighted terms for each cluster and assign sample text to the fitted clusters.

### [Topic-Modeling-LDA.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Topic-Modeling-LDA.ipynb)

Apply LDA to the prepared lecture transcripts. Inspect the terms associated with each topic and retrieve transcript passages with high weights for a selected topic.

### [LDA-Simple-Gensim.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/LDA-Simple-Gensim.ipynb)

Generate synthetic documents from word distributions related to the Cold War and economic policy. Fit an LDA model with Gensim and compare the inferred topic-word distributions with the distributions used to generate the documents.

### [Gensim-Visual-Clustering.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Gensim-Visual-Clustering.ipynb)

Explore LDA using fabricated medical research texts. Prepare a dictionary and corpus, fit a Gensim model, calculate topic coherence, and create an interactive topic visualization with pyLDAvis.

### [LDA-Document-Similarity.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/LDA-Document-Similarity.ipynb)

Generate synthetic documents from word distributions related to the Cold War and economic policy. Use cosine similarity to iteratively combine document word-count vectors, inspect the resulting word distributions, and compare the original documents with the combined representations.

### [LDA-Document-Similarity-Topics.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/LDA-Document-Similarity-Topics.ipynb)

Explore document similarity using lecture transcripts. Represent passages as word-count vectors, combine similar passages, inspect their term weights, and calculate cosine similarity between the original passages and the combined representations.

### [Topic-Similarity-BERT.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Topic-Similarity-BERT.ipynb)

Explore semantic similarity using sentence-transformer embeddings. The example compares a query passage with lecture transcript passages using cosine similarity.

### [Word-Cloud.ipynb](https://github.com/geoffswc/Topic-Modeling-Unsupervised-ML/blob/main/Word-Cloud.ipynb)

Create a word cloud from lecture transcripts after basic text preparation and stopword removal. Use the visualization to explore frequently occurring terms in the collection.

### Instructor

Geoffrey Boushey is a computational and research data science specialist at UCSF and a member of the Library’s Data Science and Open Scholarship team. He teaches courses and provides consultations on programming, data analysis, machine learning, generative AI, and computational research methods, including Python, SQL, APIs, and data visualization.
