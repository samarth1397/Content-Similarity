# Content Similarity

Let's say that we have a corpus consisting of the works of two authors. If I want to identify the regions where both the authors are talking about similar ideas or concepts, then how can this be done using computation? I'm trying to explore this idea, using standard NLP techniques. Hegel and Karl Marx are the two authors that I am using as an example, since it is already known that they spoke about similar ideas in their work. I first begin by a simple technique of document clustering. For me, a document is a small section of the book (about 1000 words that are not stop words). I will use both K-Means clustering as well as Wards clustering. I have extracted a TF-IDF vector for each document. I will also use gensim's word2vec to extract a feature vector based on the skip-gram model. 

After similar documents have been clustered together, I want to use LDA to create topic models and understand the underlying theme in these document. 
