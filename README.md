# NETFLIX-MOVIE-RECOMMENDATION-SYSTEM
This project aims to build a movie recommendation mechanism within Netflix. The dataset I used here come directly from Netflix. It consists of 4 text data files, each file contains over 20M rows, i.e. over 4K movies and 400K customers. All together over 17K movies and 500K+ customers!


<img src='http://www.techscript24.com/admin/UI/assets/img/BlogsImage/netflix-q.jpg'>

# 1. Business Problem 
## 1.1 Problem Description 
Netflix is all about connecting people to the movies they love. To help customers find those movies, they developed world-class movie recommendation system: CinematchSM. Its job is to predict whether someone will enjoy a movie based on how much they liked or disliked other movies. Netflix use those predictions to make personal movie recommendations based on each customer’s unique tastes. And while Cinematch is doing pretty well, it can always be made better.

Now there are a lot of interesting alternative approaches to how Cinematch works that netflix haven’t tried. Some are described in the literature, some aren’t. We’re curious whether any of these can beat Cinematch by making better predictions. Because, frankly, if there is a much better approach it could make a big difference to our customers and our business.

> Credits: https://www.netflixprize.com/rules.html

## 1.2 Problem Statement 
Netflix provided a lot of anonymous rating data, and a prediction accuracy bar that is 10% better than what Cinematch can do on the same training data set. (Accuracy is a measurement of how closely predicted ratings of movies match subsequent actual ratings.)


## 2.2 Mapping the real world problem to a Machine Learning Problem 
### 2.2.1 Type of Machine Learning Problem 
- For a given movie and user we need to predict the rating would be given by him/her to the movie. 
- The given problem is a Recommendation problem 
- It can also seen as a Regression problem 
### 2.2.2 Performance metric 
- Mean Absolute Percentage Error: https://en.wikipedia.org/wiki/Mean_absolute_percentage_error
- Root Mean Square Error: https://en.wikipedia.org/wiki/Root-mean-square_deviation
### 2.2.3 Machine Learning Objective and Constraints 
- Minimize RMSE.
- Try to provide some interpretability.

|Model | rmse|

|-----| ------------|

|svd         |       1.0726424481315167    |
|svdpp          |      1.0726973299570828 |
|bsl_algo       |      1.072739481395958|
|knn_bsl_u      |     1.072741563865369|
|knn_bsl_m      |   1.0728213101702937|
|xgb_final      |  1.0743198685186928|
|xgb_all_models |   1.0757537009157945|
|first_algo     |    1.076373581778953|
|xgb_knn_bsl    |   1.0784249635688925|
|xgb_bsl        |    1.079601535496083|
