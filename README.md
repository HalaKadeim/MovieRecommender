# MovieRecommender
## Description
**Movie Recommender:** is made to provide useful suggestions of movies for a streaming movies websites, it will offer personalized contents based on past behavior and it hooks the customer to keep coming back to the website. The main types of recommender algorithm are Popularity, Collaborative Filtering, Content-based Filtering and Hybrid Approaches. To short down the process Content-based Filtering will be implemented in this project. The project will try to implement the 3 programming paradigms: Imperative, functional and declarative for purposes of class requirements, to cover that Scala will be used as it is multi paradigm programming language.


##Hight Level Architecture
The following diagram shows the main compoments of the projects:
![Hight Level Architecture for Movie Recommender](https://github.com/HalaKadeim/MovieRecommender/blob/master/Images/Hight%20level%20architecture%20for%20Movie%20REcommender.png)

**Data source:** For this project will work with 10 million ratings from 72,000 users on 10,000 movies, collected by [MovieLens](http://movielens.umn.edu/).
 
**Hadoop:** since the project is designed to tackle a real world problem, and in real world in such systems data comes from multiple sources and in different structures, hadoop is necessary to store that data sources in a single place.

**Spark:** to solve low latency computing will use spark, Apache spark is an in-memory cluster computing system which provides real time data processing  capability.
 
**MLlib:** Library of machine learning will provide algorithms to build the recommendation engine which saves huge amount of time instead of building the system from scratch.

##Product Functions
Movie Recommender can be used in any movie streaming application. It collects users’ data and analyses them to come up with useful suggestion the user’s preferences.

##User Description
there will be two types of users:
 
 **1- Admin:**  is the administrator or the moderator who has full access to all the interfaces of the project (Regular Account, Updated Account, View Profile, Add a movie, Edit a movie, Delete a movie, View list of movies, Search a movie, Rate a movie, Edit movie rate, Add movie to favorites, Delete movie from favorites, Comment on a movie, Delete comment on a movie, Approve user comments).
 
**2- Regular user:** any user can access the website will have limited access to the interfaces (Regular Account, Updated Account, View Profile, View list of movies, Search a movie, Rate a movie, Edit movie rate, Add movie to favorites, Delete movie from favorites, Comment on a movie, Delete comment on a movie), this user will be the target of the recommendation system.

The Diagram below shows the use case for each user:

![Case use Diagram](https://github.com/HalaKadeim/MovieRecommender/blob/master/Images/Case%20User%20Diagram%20For%20Moive%20Recommender.png).

## Non-functional Requirements

#### Performance Requirements
Performance of making recommendation and updating this recommendation is very important issue because the system is designed to be real-timed. Means data processing should be very fast and not noticible by the user. Of course system should handle multiple users at the same time and update the recommendations after each choice the user makes.
#### Security
Database has to be reached securely and its data should not be broken. It also should not change except for the admin’s updates. Moreover, since our dataset contain some personal information of user, security design is important in the web service.
#### Usability
since the product is designed to provide service for every one, it is designed to be easily used by everyone.
