### **Observations**
1. The use of BerTopic is a game changer and has its power in the Topic modelling.
2. With the use of topic modelling, the documents could be grouped together to gain more insight into the data.
3. For reproducibilty purposes, the sentence tranformer was passed into the embedding_model so as to allow the saved model to be used on test data.
4. Outliers were removed and redistributed into other topics, moreover all other topics which showed some level of similarity was merged into a singular topic for better representation purposes.
5. Again to understand why a single document is assigned to a particular topic, the topic distributtion was calculated on a token level to see why the words are heavily likely to belong a topic(s).
6. Further analysis could be done with the documentations such as; 
    - [Guided Topic Modelling](https://maartengr.github.io/BERTopic/getting_started/guided/guided.html)
    - [Dynamic Topic Modeling](https://maartengr.github.io/BERTopic/getting_started/topicsovertime/topicsovertime.html)
    - [Supervised Topic Modeling](https://maartengr.github.io/BERTopic/getting_started/supervised/supervised.html)
    - [Semi-supervised Topic Modeling](https://maartengr.github.io/BERTopic/getting_started/semisupervised/semisupervised.html)
    - [Hierarchical Topic Modeling](https://maartengr.github.io/BERTopic/getting_started/hierarchicaltopics/hierarchicaltopics.html#linkage-functions)
    - [Online Topic Modeling](https://maartengr.github.io/BERTopic/getting_started/online/online.html)
    - [Manual Topic Modeling](https://maartengr.github.io/BERTopic/getting_started/manual/manual.html)