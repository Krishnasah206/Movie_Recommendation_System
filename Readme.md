# Movie Recommendation System

This project is a web-based movie recommendation system using Streamlit for the frontend. It utilizes The Movie Database (TMDB) API and a machine learning model to recommend similar movies based on user input.

## Features
- Select a movie from a dropdown list.
- Get 5 similar movie recommendations.
- See the poster of each recommended movie, fetched from the TMDB API.

## Dataset
The project uses the TMDB 5000 Movies and TMDB 5000 Credits datasets, which are included in the repository as CSV files.

## Technologies Used
- **Streamlit** for the frontend UI.
- **Pandas** for data handling.
- **Pickle** for loading pre-trained models and data.
- **TMDB API** for fetching movie posters.
- **Machine Learning** for recommending movies based on similarity.

## How to Run the Project

### 1. Clone the repository:
```bash
git clone https://github.com/yourusername/movie-recommender-system.git
cd movie-recommender-system
```

### 2. Install the required libraries:
```bash
pip install streamlit pandas requests
```

### 3. Run the application:
```bash
streamlit run app.py
```

<img src='./img.png' alt="Image">

### 4. How it works:
- The system uses a pre-trained similarity matrix stored in `similarity.pkl` to find similar movies.
- The movie data is loaded from `movie_dict.pkl`.
- When a user selects a movie, the system recommends 5 movies and displays their posters.

## Files in the Repository
- `app.py`: Main Streamlit application.
- `movie_dict.pkl`: Pickled file containing movie data (title and movie_id).
- `similarity.pkl`: Pickled file containing the pre-trained similarity matrix.
- `tmdb_5000_credits.csv`: Dataset containing movie credits.
- `tmdb_5000_movies.csv`: Dataset containing movie details.

## TMDB API
This project uses TMDB API to fetch movie posters. You will need to use your API key in the project. Make sure to keep it secure by not hardcoding it into your source code (or store it in environment variables).

## Future Enhancements
- Add more filtering options (e.g., genre, year).
- Improve recommendation algorithms with more advanced models like collaborative filtering.
- Handle edge cases where movies do not have a poster available.

