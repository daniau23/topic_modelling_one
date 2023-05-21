## **Topic Modelling**
### **What is topic modelling**

Topic modelling is an unsupervised learning technique used in text analytics, NLP (Natural Language Processing) or machine learning for the purpose of discovering topics or themes which exists in a large corpus (a collection of documents) leading to the extraction of useful insights, patterns and relationships.

### **Summary of project**
- The project begins with the text analytics of the scraped tweets via Tweepy & Twitter API.

- The scraped tweets was preprocessed in order to remove unwanted stop words and redundant text such as digits, hyperlinks, punctuations, etc, before applying the LDA model (Latent Dirichlet Allocation) approach which would generate the topics. 
    - Bigrams approach was first used and it yielded 6 topics namely;
        - Topic 0: AI & healthcare
        - Topic 1: sports 
        - Topic 2: politics
        - Topic 3: sports
        - Topic 4: disaster
        - Topic 5: politics and AI
    - Trigrams approach was also used adn it reduced the topics size from 6 to 4 topics. But was it truly worth it?
        - Topic 0 is about sports.
        - Topic 1 is about politics.
        - Topic 2 is about AI and healthcare.
        - Topic 3 seems to be about sports and politics? Should it be a general topic?
    
        It somewhat captures the relevance of each document to each topic cluster. I believe this could be improved through the following:
        - The Phrase formation.
        - The filtering of the extremes.
        - TF-IDF could also be used in the preprocessing phase.
        - Using other topic coherence evaluation techniques.

- The Top2Vec approach was applied to the sracped tweets. The algorithm takes care of the preproccessing as it generates the topics for us.
    - Version1 of the approach made use of **doc2vec** embeddings approach was had topic size of 46 topics.
    - Version2 made use of **transformer** embeddings which was downlaoded and applied. It had a topic size lower than the doc2vec approach; 35 topics.
    - Version3 still involved using doc2vec approach but  allow the use of hierarchical_topic_reduction() method to reduce  46 topics to 6 topics.

- Finally, the BerTopic approach, **BERTopic is a topic modeling technique that leverages 🤗 transformers and c-TF-IDF to create dense clusters allowing for easily interpretable topics whilst keeping important words in the topic descriptions.** 
    - One thing about BerTopic is that it's [modular](https://maartengr.github.io/BERTopic/algorithm/algorithm.html#code-overview), meaning you could construct your particular BerTopic in a form that suits your specification/appraoch.
    - The model can be saved and used on new textual data to predict which topic it falls under based off the pretrained model on the training data.
    - Topics identified:
        - Topic 0 is related to USA and politics
        - Topic 1 is related to sports.
        - Topic 2 is related to AI and healthcare.
        - Topic 3 is related to disaster/disease.
        - Topic 4 is related to Nigeria and politics.

### **Replicating this project**

Dependencies for this project can be found in env.yml

1. Download and install &nbsp;[Anaconda](https://www.anaconda.com/products/distribution#Downloads)

2. Navigate to your desktop and create a new folder using  **mkdir "folder_name1"** and paste the env.yml file into **folder_name1** 

3. Create another folder within folder_name1; **folder_name1/folder_name2**

4. Run **conda env create -f env.yml -p ../folder_name1/folder_name2**

5. Run **conda env list** to list all environments created using Anaconda

6. Run **conda activate ./folder_name2** to activate the environment

7. Run **conda list** to check if all dependencies have been installed

8. Have fun experimenting !

