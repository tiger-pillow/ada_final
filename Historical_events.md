### Doc2Vec description

To compare historical events and their relationship to movies, 
a method for finding similarities between the films and events is required. Doc2Vec is an appropriate method for vectorizing an arbitrary-size document, enabling the computation of cosine similarity between two documents in the vector space. For our purpose of finding similarities between movies and events, a Doc2Vec model is created based on the plot summaries in our dataset. By vectorizing the descriptions of events, we can now find the films with the lowest cosine similarities, thus most similar characterizations to our event.

![image](https://user-images.githubusercontent.com/47889649/209131181-8d2be2d4-1dbc-42f3-907b-78923caf9f82.png)
With regards to above metric, here is the distrbution of similarities between events and movies.

### explain how we got the events, and event summary

The events used in the following analysis were taken from "https://www.historyonthenet.com/20th-century-timeline", where the most relevant onces were hand-picked ones. Since we would like the descriptions of the movies and the events to come from the same source however, the event's corresponding Wikipedia description was used when finding similarities to the movie plot summaries.


### explain lemma and stop words
When vectorizing the movie summaries and event descriptions for comparison, it is good practice to extract only the essence of the texts before the vectorization. Therefore the stopwords, which frequently occur in different documents, are removed. Additionally, lemmatization was done on these documents to group words with the same canonical form, e.g., "go" and "going". 





![image](https://user-images.githubusercontent.com/47889649/209132199-77a2801e-1db1-4ac9-a39d-b8e27510ea9c.png)
After events occured there the fraction of movies similar to events increased. The fractions are calculated by taking the number of similar movies before/after an event occured, divided by the total number of movies made before/after event occured
