# MovieRecommendationSystem
 This is a content-based Movie Recommendation System built using Python and machine learning libraries. The system suggests movies based on similarity of features such as genre, keywords, tagline, cast, and director.

## Features

- Content-based filtering using movie metadata
- Movie similarity calculated using TF-IDF and Cosine Similarity
- Input a movie name and get similar movie recommendations
- Handles missing values in metadata gracefully

## Technologies Used

- *Programming Language:* Python
- *Libraries:*
  - pandas – data manipulation
  - numpy – numerical operations
  - scikit-learn – TF-IDF Vectorization and Cosine Similarity
  - difflib – finding close matches for user input

## Dataset

*Source:* movies.csv (from TMDB or similar open-source movie metadata datasets)
- *Size:* 4803 movies with 24 columns of metadata
- *Selected Features for Recommendation:*
  - genres
  - keywords
  - tagline
  - cast
  - director

## How It Works
1. *Data Preprocessing:*
   - Load movie dataset
   - Select key metadata features
   - Replace missing values with empty strings
   - Combine all selected features into a single string

2. *Feature Vectorization:*
   - Use TfidfVectorizer to convert text data into numerical feature vectors

3. *Similarity Measurement:*
   - Compute cosine similarity between all movies based on their feature vectors

4. *Recommendation:*
   - Take user input (movie title)
   - Find the closest matching title
   - Recommend top N most similar movies based on cosine similarity

## How to Run
This project runs best in *Google Colab*.

### Run on Colab

1. Open the notebook:  
   [*Open in Google Colab*](https://colab.research.google.com/github/Sourav-10x/movie-recommendation-system/blob/main/Movie_Recommendation_System.ipynb)

2. Upload the movies.csv file when prompted.

3. Run all the cells and enter a movie name when asked.

---

### Optional: Run Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/Sourav-10x/movie-recommendation-system.git
   cd movie-recommendation-system
2. Install requirements:
 pip install -r requirements.txt
3. Open the Jupyter Notebook:
 jupyter notebook

**Example Usage**

Enter your favourite movie name : Iron Man

Recommended movies:
1. Iron Man 2
2. Avengers: Age of Ultron
3. Captain America: The First Avenger

## License

This project is licensed under the [MIT License](LICENSE).

You are free to use, modify, and distribute this project for personal or commercial purposes, provided that proper credit is given to the original author.
...
