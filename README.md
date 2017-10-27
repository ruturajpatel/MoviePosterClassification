# MoviePosterClassification

We examined multi-label classification model to identify genres associate with movies using their posters. As the dataset was not readily available, we crawled around 29000 posters from IMDB database. Using the Inception V3 model we extracted the high-level features from 300x300 pixel colored poster image which were input to the 3 fully connected layers and 1 output layer, an extension to the base model. The output was in form of hot encoded vector with sigmoid activation function in final layer of the network to achieve multi-label classification. Eventually, we analyzed the classification problem as an information retrieval problem to predict top 10 relevant posters based on the genre. Also, we developed a user-interface in which a user can upload a poster and the system will predict the genres that can be associated with the given poster. The system uses the trained weights after training the algorithm with around 5000 images which predicts all the genre correctly for almost 70% of the uploaded posters.

## Overview

Movie information sites such as IMBD, Rotten Tomato are well-known for its huge database
of movies and movie reviews. These sites often classify and recommend movies based on
genres. However, this process is prone to error as the genre labeling for movies is based on the user suggestions and people often misunderstand the context or story, leading to wrong genre categorization. To overcome such inaccuracies associated with the classification of movies, it is very important to automate the process of the genre labeling using an algorithm that is far more accurate than a human being. Many researchers have studied the problem of automatic genre classification using textual movie attributes such as title, user reviews, and audio visual features of a movie such as trailers.

People often judge a book by its cover and same is the case for movie posters. People generally infer certain information about the movie by looking at a movie poster and often  judge whether to watch a movie based on their initial impression of a movie poster. Thus, movie producers often try to make movie posters which resembles to nature of the movie so that the poster can grab attention and attract audience. Hence, movie posters can be an important element in labeling the genres associated with it. In this project, we aim at creating a classification system that can assign genres to a movie given its poster. It can also be treated as an information retrieval problem that can classify and recommend movies to user based on its genres. Using the results of this research, we aim to study how low level features of the poster such as color, text and objects can affect the movie categorization problem.

Classifying a movie using its poster is a computer vision problem commonly described as assigning labels to an image. Most of solutions encourage single label classification. The fundamental problem with the automatic genre classification of movies is that it is a multilabel classification problem as more than one genre could be assigned to a single movie. It is important to implement such system with higher accuracy as it could help to improve quality of an online movie database and provide preference based recommendations to users.
