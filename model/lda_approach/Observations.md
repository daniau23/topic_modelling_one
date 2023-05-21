### **Observations**
1. After careful examination, trigrams does reduce the number of clusters (topics) needed to 4. 
2. It somewhat captures the relevance of each document to each topic cluster. I believe this could be improved through the following:
    - The Phrase formation.
    - The filtering of the extremes.
    - TF-IDF could also be used in the preprocessing phase.
    - Using other topic coherence evaluation techniques.
3. The topic clusters are majorly talking about the following:
    - Topic 0 is about sports.
    - Topic 1 is about politics.
    - Topic 2 is about AI and healthcare.
    - Topic 3 seems to be about sports and politics? Should it be a general topic?

4. The use of bigrams does capture the coherence of each document to each topic, about 6 topic/clusters should be used for this.
5. The topic clusters are majorly talking about the following:
    - Topic 0: AI & healthcare
    - Topic 1: sports 
    - Topic 2: politics
    - Topic 3: sports
    - Topic 4: disaster
    - Topic 5: politics and AI