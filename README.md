# Embedding
Natural language processing systems use modern distributional semantic algorithms, also known as
word embedding algorithms, to learn meaningful vectors for words. The aim of these algorithms is to create
embeddings in such a way that words with similar meanings have similar mathematical representations.
Word embeddings can be categorized into two broad categories: frequency-based and prediction-based.

We implement a frequency-based embedding modelling approach - Singular Value Decomposition (SVD), and compare it with the embeddings obtained using one of the variants of Word2vec - CBOW implementation with Negative Sampling. The analysis will highlight the differences in the quality of embeddings obtained.  

Model was trained on: https://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Movies_and_TV.json.gz

# Implementation
## 1) SVD by building co-occurance matrix
a.ipynb contains the code for implementation of word embedding model and train word vectors by first building a Co-occurrence Matrix, followed by the application of SVD.

svd_emb.txt contains the embeddings generated through this model. It can be found in the following google drive link.
https://drive.google.com/file/d/15CNUQVREoV-qvN5QYcnu8ADqKKqHvI98/view?usp=sharing

## 2) word2vec using cbow with negative sampling
b.ipynb contains the code for implementation of word2vec through cbow with negative sampling.

cbow.txt contains the embeddings generated through this model.

# Analysis
- part1: Display top-10 word vectors for five different words (a combination of nouns, verbs, adjectives, etc)  
- part2: Finding the top 10 closest words for the word ‘titanic’ and 'water'
a_analysis.ipynb contains the code for part 1 and 2 of analysis of SVD embeddings.
b_analysis.py contains the code for part 1 and 2 of analysis of word2vec embeddings.

# Note:
All the above files were run on google colab and have been directly downloaded from google drive. The dataset given was uploaded to the drive and was used from there for the code and model implementation. 

So to run the code, you will have to upload the dataset (unzipped) to drive, upload the .ipynb files in colab, and run the code.
