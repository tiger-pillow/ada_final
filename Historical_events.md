*** Doc2Vec description
To compare historical events and their relationship to movies, 
a method for finding similarities between the films and events is required. Doc2Vec is an appropriate method for vectorizing an arbitrary-size document, enabling the computation of cosine similarity between two documents in the vector space. For our purpose of finding similarities between movies and events, a Doc2Vec model is created based on the plot summaries in our dataset. By vectorizing the descriptions of events, we can now find the films with the lowest cosine similarities, thus most similar characterizations to our event.

