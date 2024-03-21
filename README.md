# Movies-Topic-Modelling

Topic Modeling has been a common technique in identifying topics within textual data. Large tech companies have only very recently employed explicit topic modeling in their sophisticated reviews systems. Movie reviews can be difficult to analyze on a large scale due to the focus on specific actors or plot elements that can shroud overall themes. This project present an unsupervised model pipeline that can extract themes from movies and calculate an approximate overall sentiment for each theme. This is similar to Google Reviews or Amazon's new feature in finding qualities in products from reviews.

For example, passing a movie like Shawshank Redemption may produce topic categories such as 'Acting,' 'Cinematic Production,' 'Character Development,' 'Friendship,' 'Hope,' etc. and provide each with a sentiment analysis score. BERTopic was the primary library used for topic modeling, OpenAI's Completion API was used to assign simple labels to textual clusters, and NLTK was used for sentiment analysis. 

The utilization is as simple as entering a specific movie name and a sentiment chart for each topic will be outputted.

KEY INSIGHT: 
In our model, we arbitrarily split review texts into chunks of 3 sentences or less. This was because reviews often contain many themes, which would be difficult to assign one single theme to the original review. While arbitarily splitting may cut into context that the review originally had, BERTopic is well fitted for this because these 'out-of-context' segments are removed when forming topic clusters.

However, it was found to be important in conducting sentiment analysis on the original document and tie it to all its text segments rather on those text chunks. It still often produced great results as it was found that individuals tend to mention elements that match their overall sentiment of the movie (i.e. skip over the negative elements if they highly enjoyed the movie).


Example run() for Avengers Endgame:

<img width="475" alt="Screenshot 2024-03-20 at 10 28 01 PM" src="https://github.com/michael-L-i/Movies-Topic-Modelling/assets/59122382/35436b42-a156-4be2-9607-3627c6796c66">
