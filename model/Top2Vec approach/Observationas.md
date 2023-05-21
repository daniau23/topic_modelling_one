### **Observations**
1. Version1 had a topic size of 46 topics but version2 had a topic size of 36 topics, which shows an improvement of the algorithm when using a transformers embeddings than using doc2vec embeddings. 
2. In version3, the method hierarchical_topic_reduction() was used to reduce the number of topics from 46 topics to 6 topics. This reduced the redunacy and overfitting by the algorithm. 
3. Once the hierarchical_topic_reduction() is applied to the algorithm, it saves the reduced number to be made used of within other methods.