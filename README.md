# EODS-Project2-Group9
 
### NLP pipeline with sentiment prediction
* Tokenization
    > Split text into tokens(sentences or words), for this question, we split the document into sentence for automatic summarization, and words for sentiment analysis and topic modeling
* Screen out stop words and other meaningless corpus
* Lemmatization
    > Here we only use lemmatization rather than stemming is because lemmatization keeps the interpretability of words with their context. While stemming might lead to incorrect meaning. 
* EDA: wordCloud with different sentiment
    > Identify what poeple with different emotions were considering about
* EDA: Word2vec with Clustering
    > Word2Vec: Effective for detecting the synonymous words or suggesting additional words for a partial sentence

    Clustering methods: K-means + DBScan
    
    Use all the words in a specific part-of-speech from all the documents (e.g. all nouns / all adj.s)
* Topic Modeling: Feature extraction by TFIDF + Latent Dirichlet Allocation
    > Build a pipeline with kFoldCV to find the best topic number
* Automatic summrization
    > Identify what were most people thinking about or tweeting for
* Sentiment Analysis: Classification for sentiment(5 classes: Neutral / Positive / Extremely Positive / Negative / Extremely Negative)
    > Potential Model: BERT?