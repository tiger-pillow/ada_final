### Doc2Vec description

To compare historical events and their relationship to movies, 
a method for finding similarities between the films and events is required. Doc2Vec is an appropriate method for vectorizing an arbitrary-size document, enabling the computation of cosine similarity between two documents in the vector space. For our purpose of finding similarities between movies and events, a Doc2Vec model is created based on the plot summaries in our dataset. By vectorizing the descriptions of events, we can now find the films with the lowest cosine similarities, thus most similar characterizations to our event.

### explain how we got the events, and event summary

The events used in the following analysis were taken from "https://www.historyonthenet.com/20th-century-timeline", where we hand-picked the most relevant ones. Since we would like the descriptions of the movies and the events to come from the same source, the event's corresponding Wikipedia description was used when finding similarities to the movie plot summaries.


### explain lemma and stop words
When vectorizing the movie summaries and event descriptions for comparison, it is good practice to extract only the essence of the texts before the vectorization. Therefore the stopwords, which frequently occur in different documents, are removed. Additionally, lemmatization was done on these documents to group words with the same canonical form, e.g., "go" and "going". 





