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
- Load the dataset named "Movie_ID_Titles" from a CSV file using the Pandas library.
- Now load the second one which is "u.data" which contains ratings corresponding to item_id and user_id.
- Let's merge both dataframes together so we can have ID with the movie name.

--> Step-2: Data Visualization
- 
