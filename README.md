# Text-Summarization
Text summarization machine learning model
This method includes text summarization on the basis of occurance of certain words in the article .
The occurance of words are associated with a rank of the sentence which gives the sentence a higher probability to occur in the summary.
NLTK has been used for for sentiment analysis.

#Text summarization can broadly be divided into two categories — Extractive Summarization and Abstractive Summarization.#

Extractive Summarization: These methods rely on extracting several parts, such as phrases and sentences, from a piece of text and stack them together to create a summary. Therefore, identifying the right sentences for summarization is of utmost importance in an extractive method.
Abstractive Summarization: These methods use advanced NLP techniques to generate an entirely new summary. Some parts of this summary may not even appear in the original text.

TextRank Algorithm
Let’s understand the TextRank algorithm, now that we have a grasp on PageRank. I have listed the similarities between these two algorithms below:

In place of web pages, we use sentences
Similarity between any two sentences is used as an equivalent to the web page transition probability
The similarity scores are stored in a square matrix, similar to the matrix M used for PageRank
