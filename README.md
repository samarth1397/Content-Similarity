# Content Similarity 

Using the works of Karl Marx and Hegel as an example, I want to understand, how can we identify regions of their work where they both talk about similar ideas and topics. I will start with a naive approach of document clustering based on TF-IDF vectors. I would use smaller sections of the books as documents, i.e. one document would consist of about 1000 context words (or not stopwords). 

Once I have identified similar documents using clustering algorithms, I would like to perform topic modelling on these specific documents and then compare the topics generated. 
