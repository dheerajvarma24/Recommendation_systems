# Recommender Systems

The technique used in recommender systems is Collaborative Filtering. There are two types of Collaborative Filtering techniques.

### 1) User based Collaborative Filtering: Grouping users of similar interests and recommending stuff from other person likes in the same group which I haven't seen yet.

#### Working intuition:

Build a matrix of things that a user has bought / viewed / rated. ( rows - users, cols - items)

Computer similarity score. Simple dot product or pesrson corrleation score. Find similar users and recommending stuff that other users has bought.

#### Limitations:

* People interests changes over time.

* One can create Fake users ( shilling attack) and manipulate results.



### 2) Item based Collaborative Filtering:  Grouping similar items together

#### a. Naive way: group items based on Genre, language, year etc.

#### b. CF: group items based on user ratings.

Consider 2 movies at a time. Find all the users who have rated both the movies and compute the movies similarity score and if they are similar, group those items. (same as 1 but rows and cols flipped while calculating similarity.) 

#### Limitations:

* If it is a new item and has no reviews then it is not possible to generate similar items.

* Computationally expensive

