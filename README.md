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

Introduction to Sequence-to-Sequence (Seq2Seq) Modeling
We can build a Seq2Seq model on any problem which involves sequential information. This includes Sentiment classification, Neural Machine Translation, and Named Entity Recognition – some very common applications of sequential information.

In the case of Neural Machine Translation, the input is a text in one language and the output is also a text in another language:

nmt

In the Named Entity Recognition, the input is a sequence of words and the output is a sequence of tags for every word in the input sequence:

ner

Our objective is to build a text summarizer where the input is a long sequence of words (in a text body), and the output is a short summary (which is a sequence as well). So, we can model this as a Many-to-Many Seq2Seq problem. Below is a typical Seq2Seq model architecture:

seq2seqThere are two major components of a Seq2Seq model:

Encoder
Decoder
Let’s understand these two in detail. These are essential to understand how text summarization works underneath the code. You can also check out this tutorial to understand sequence-to-sequence modeling in more detail.

 
