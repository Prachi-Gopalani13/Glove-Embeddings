# Glove-Embeddings

## Explaination in my Blog:
https://medium.com/ai-in-plain-english/implementation-of-pre-trained-glove-word-embeddings-on-dataset-dceb141297c9

## Data
https://github.com/Prachi-Gopalani13/Glove-Embeddings-LSTM-Disaster-Tweets/tree/main/Data

## The GloVe Model
The statistics of word occurrences in a corpus is the primary source of information available to all unsupervised methods for learning word representations, and although many such methods now exist, the question still remains as to how meaning is generated from these statistics, and how the resulting word vectors might represent that meaning.

GloVe observes that ratios of word-word co-occurrence probabilities have the potential for encoding some form of meaning. Take the example from StanfordNLP (Global Vectors for Word Representation), to consider the co-occurrence probabilities for target words ice and steam with various probe words from the vocabulary.

## Word2Vec vs GloVe
Word vectors put words to a nice vector space, where similar words cluster together and different words repel. The advantage of GloVe is that, unlike Word2vec, GloVe does not rely just on local statistics (local context information of words), but incorporates global statistics (word co-occurrence) to obtain word vectors.

## Imports
We’re going to need to use, Numpy, Scipy, Matplotlib, and Sklearn for this project.

## Data Cleaning
1) Removing URLs
2) Removing HTML tags
3) Removal of Punctuations

## Padding Sentences
Allocating 50 word as length for ever sentence. Tokenising every word of the corpus and later padding the sentence to the MAX_LEN allocated i.e. 50 words per sentence.
