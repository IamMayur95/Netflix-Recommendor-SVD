# Netflix-Recommendor-SVD
Netflix-Recommendation-Engine
Below are the 3 objectives for this project:
1.	Find out the list of most popular and liked genre
2.	Create Model that finds the best suited Movie for one 
user in every genre.
3.	Find what Genre Movies have received the best and 
worst ratings based on User Rating.
Steps performed to achieve the objectives above: (Unable to commit the dataset due to its size)
1.	Originally dataset – ‘combined_data_1.csv’ consisted data in the format:
a.	1: --> Represents Movie Id
b.	After that 1st value represents Customer_id
c.	2nd value represents Rating given by that customer to that movie
d.	3rd value represents the year

2.	Transformed the data from dataset – ‘combined_data_1.csv’ in the format as below:
 

3.	In order to reduce the size of data set , removed the less rated movies . Also, removed the data of customers who have rated less. (Only top 30% considered)
4.	Create ratings matrix for 'ratings' matrix with Rows = Cust_Id, Columns = Movie_Id
 
5.	Loaded another dataset with movie details – ‘movie_titles _1_.csv’
6.	Created an SVD model and evaluated its metrics as below
 

7.	Trained the SVD model for a single user and predicted the score for movies to recommend to that user.
 

8.	Then found the User to Concept Similarity Matrix and Movie to Concept Similarity Matrix.
9.	Then based on Movie to Concept matrix we found the best and worst movie for a Genre
 

