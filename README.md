# Movie-Recommendation-System
This is a Content-Based and Popularity-Based Movie Recommendation System created using Python. The system utilizes movie metadata and generates personalized recommendations based on cosine similarity.

# Features
- **Content-Based Recommendation:** Suggests movies similar to a user's favorite movie based on metadata like genres, keywords, tagline, cast, and director.
- **Similarity Calculation:** Uses TF-IDF Vectorization and Cosine Similarity to compute similarity scores between movies.
- **Popularity Factor:** Ensures that well-known movies are highlighted during recommendations.
- **Interactive Input:** Accepts user input for their favorite movie and provides suggestions dynamically.

# Dataset
The system uses a CSV file (movies.csv) containing metadata for movies, including:

- Title
- Genres
- Keywords
- Tagline
- Cast
- Director

# Code Explanation
## Data Preprocessing
**Null Value Handling:** Replaces missing values in genres, keywords, tagline, cast, and director with empty strings.
**Feature Engineering:** Combines selected metadata features into a single string for each movie.
## TF-IDF Vectorization
Converts the combined features into a numerical representation using TF-IDF vectorization.
Reduces the weight of commonly occurring words to improve similarity calculations.
## Cosine Similarity
Measures the similarity between two movie vectors.
Generates a similarity matrix that serves as the basis for recommendations.
## Recommendation Generation
Finds the closest matches to the user's input using difflib.
Retrieves movies with the highest similarity scores from the matrix.

# Example
 Enter your favourite movie name: Titanic
 
 Movies suggested for you:
 
 1 - Romeo + Juliet
 
 2 - Pearl Harbor
 
 3 - The Notebook
 
 4 - The Great Gatsby
 
 5 - Avatar
