# Movie-Recommender-System

# PROBLEM STATEMENT
- Recommender systems are used to suggest movies or songs to users based on their interest or usage history.
- For example, Netflix recommends movies to watch based on the previous movies you've watched.
- In this example, we will use Item-based Collaborative Filter

# PROJECT OVERVIEW:
-- First of all,we need to check whether it is regression task or classifiction task...
        
    It is a classification task as we have to classify whether user liked the specific movie or not.
-- Here,we are going to  use itmem-based collaborative filtering. This works by recommending elemnents based on relationship between items and not on user(people).
If we do filtering based on user there are some limitations like user tastes can be change time to time and there are more users than product(movie) so which makes it complex. And item taste will not change ,it is constant.So,we do Item-based collaborative filtering.

# STEPS TAKEN:

So,here are the step I followed in this problem statement:

--> Step-1: Importing the libraries.
- Begin by importing essential libraries such as NumPy for basic calculations, Pandas for handling dataframes, Matplotlib for plotting graphs, and Seaborn for visualizing data.

--> Step-2 Load the datast.
- Load two datasets: "Movie_ID_Titles" contains information about movie titles, and "u.data" contains user ratings corresponding to item_id and user_id. 
- Merge these datasets to create a comprehensive dataframe with both movie names and ratings.

--> Step-3: Data Visualization
- Create datasets, 'rating_df_count' and 'rating_df_mean,' listing movie titles along with their ratings based on count and mean, respectively.
-  Combine these two datasets into 'rating_mean_count_df.
- Visualize the distribution of mean ratings and rating counts using histograms
- Sort movies by mean rating and count to identify highly-rated movies with substantial reviews.
  
--> Step-4: Perform Item-Based Collaborative Filtering On One Movie Sample
- Generate a user-movie matrix using a pivot table, showcasing how users have rated various movies.
-Select a movie sample, like 'Titanic,' and find correlations between 'Titanic' and other movies.
- Filter the correlation vector, discarding movies with fewer than 80 reviews, to ensure meaningful correlations.

--> Step-5: Create an Item-Based Collaborative Filter on Entire Dataset
- Calculate correlations between all movies in the dataframe using the Pearson method. 
- Create our own dataframe with our own ratings named 'My_Ratings.csv'.
- Now we make a list of similar movies i have rated with almost same ratings.
- Then sort the list according to correlations and recommend the most similar movie to user.
