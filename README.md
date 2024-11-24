# Movie Recommendation System 🎥✨

**Overview**
This Movie Recommendation System suggests movies to users based on their favorite movie title. It uses content-based filtering, a machine-learning technique that leverages movie similarity scores to recommend titles similar to the user's input. This project demonstrates how to preprocess movie datasets, calculate similarity scores, and provide personalized recommendations.

**Features**
User Input: Users enter the name of their favorite movie.

Closest Match: The system identifies the closest matching movie title using string similarity.

Movie Recommendations: Based on the selected movie, the system calculates similarity scores and provides the top 10 recommendations.

Efficient Search: The system handles minor spelling variations and ensures recommendations even if the input isn’t exact.

**How It Works**
**Input and Matching:**
The user enters a favorite movie title. The system uses the difflib.get_close_matches function to find the closest match from the dataset of movie titles.

**Finding Movie Index:**
The movie ID of the closest match is retrieved from the dataset to use in similarity score computations.

**Similarity Computation:**
Precomputed similarity scores (e.g., cosine similarity) between movies are used to identify how similar each movie is to the selected movie.

**Ranking and Sorting:**
The system ranks all movies based on their similarity scores, sorts them in descending order, and extracts the top 10 recommendations.

**Output:**
The top 10 movies are displayed, showing the most relevant recommendations.

**Technologies Used**
**Python**: For data processing and implementation.
**Pandas**: To handle and manipulate the movie dataset.
**difflib**: For finding close matches to user input.
**Scikit-learn**: For calculating similarity metrics.
**Prerequisites**
Install Python 3.6 or higher.
Install required libraries:
_pip install pandas scikit-learn_
