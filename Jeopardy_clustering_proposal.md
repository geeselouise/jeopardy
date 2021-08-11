# Jeopardy Questions: Topic Modeling

Louisa Reilly

## Design:
Jeopardy is an American TV game show that features a quiz competition where the contestants are presneted with general knowledge clues as answers, and they have to rephrase their responses in a question format. Contestants historically study intensively for the competetion by quizzing themselves on previous questions and learning about a wide variety of different topics. The show emphasizes breadth over depth, as well as certain topics such as art, history, pop culture, science etc. Each question set has its own niche category.

I am interested in separating out the very niche categories of Jeopardy questions into more general subjects via clustering. First, topic modeling will be done. Afterwards, a clustering algorithm will be applied.

## Data:
A set of over 200,000 [Jeopardy questions](https://www.reddit.com/r/datasets/comments/1uyd0t/200000_jeopardy_questions_in_a_json_file/) posted on the subreddit r/datasets.
They were obtained via webcrawling on [J! Archive](https://www.j-archive.com/) by the reddit user *u/trexmate*.
- Exactly 216,930 questions and answers are in this dataset.
- In addition to the questions and answers, each row one has their category, $ value, round, show number, and air date.
- The dataset needs to be cleaned as there are some html tags present.
Since the reddit post is 8 years old, I also plan to scrape [J! Archive](https://www.j-archive.com/) to obtain the more recent Jeopardy question data. 

## Algorithms:
- Topic modeling will be done using Latent Derelicht Analysis. 
- Clustering via K-means.
- For the visualizations t-distributed stochastic neighbor embedding (TSNE) will be used.

## MVP:
- Document-term, Document-topic, Topic-term matrices.


## Tools: 
- Python text processing librariers: NLTK, spaCy, gensim, and scikit-learn.
- Numpy and pandas will be used for some of the processing.
- Visualization via Tableau and some use of seaborn/ matplotlib.