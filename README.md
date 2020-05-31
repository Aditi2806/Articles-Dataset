# Text Summarization

This repository contains 3 different approaches in implementing Text Summarization. The first method is using basic modules and functions provided by the NLTK library. This method produces an extractive summarization of the text, which includes ranking the sentences present in text and selecting top N sentences for the summary.

The next method makes use of TextRank algorithm which is based on the PageRank algorithm developed by Google to rank webpages. Similar to the algorithm, TextRank also works on a similar principle, instead it ranks sentences present in the text by using the cosine similarity scores between various sentences. This method also produces extractive summarization.

To implement abstractive or human like summaries of the text, Sequence-to-Sequence model was used, which contain an encoder-decoder architecture to generate the summaries based on the input. It follows supervised method of learning and is therefore trained on the 'news_summary' dataset. The encoder takes in the input data, preprocesses it and converts in into an encoded sequence to be fed into the decoder. The decoder takes in the encoded sequence and generates the decoded sequence, which in this case is the summary of the input text.
