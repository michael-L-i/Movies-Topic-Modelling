# Movies-Topic-Modelling

Topic Modeling has been a common technique in identifying topics within textual data. Large tech companies have only very recently employed explicit topic modeling in their sophisticated reviews systems. Movie reviews can be difficult to analyze on a large scale due to the focus on specific actors or plot elements that can shroud overall themes. This project present an unsupervised model pipeline that can extract themes from movies and calculate an approximate overall sentiment for each theme. This is similar to Google Reviews or Amazon's new feature in finding qualities in products from reviews.

For example, passing a movie like Shawshank Redemption may produce topic categories such as 'Acting,' 'Cinematic Production,' 'Character Development,' 'Friendship,' 'Hope,' etc. and provide each with a sentiment analysis score. BERTopic was the primary library used for topic modeling, OpenAI's Completion API was used to assign simple labels to textual clusters, and NLTK was used for sentiment analysis. 

The utilization is as simple as entering a specific movie name and a sentiment chart for each topic will be outputted.
