# Content Similarity 

If I want to explore the works of two authors (can be extended to multiple) to identify regions of their work where they may be talking about similar ideas or topic, how can this be done? I will be using Karl Marx and Hegel as my authors since it is known that they spoke about similar ideas in certain sections of their work. To tackle this problem, I begin by clustering their works that have similar features. I have broken their works into smaller sections, following which TF-IDF vectors will be extracted from each section (I will also use Gensim's doc2vec approach which is based on the skip-gram model). Once we have a feature vector for each section, we can use K-Means clustering (We will use a variety of K's). 

After we have identified similar sections, we can use topic modelling only on these sub sections to extract the topics in this part of the work. We can then compare the topics generated using similarity measures such as Jaccard and Cosine. 
