# Movie Recommender System

This project is a web-based application for recommending movies. 
We cleaned the dataset, transformed, did feature extraction, text processing, vectorization and  
leveraged cosine similarity to suggest movies based on user input. The app is built 
using Python and Streamlit, with data fetched dynamically from The Movie Database (TMDb) API.

## Project Structure

```bash
├── app.py                  # Main Streamlit application script
├── movie_recommender.ipynb # Jupyter Notebook for model development and experimentation
├── src/                    # Source code folder (helper functions and modules)
├── artifacts/              # Serialized data files (movie_list.pkl and similarity.pkl)
├── requirements.txt        # List of dependencies
└── README.md               # Project documentation
```
## Features

- **Cosine Similarity**: Uses similarity scores to recommend movies.
- **Dynamic Data Fetching**: Fetches movie posters and details in real-time using the TMDb API.
- **Interactive UI**: Simple, user-friendly interface built with Streamlit.

## Getting Started
### Prerequisites

- Python 3.7+
- Access to the internet for fetching data from the TMDb API.

### Installation
1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/movie-recommender-system.git
cd movie-recommender-system
```
2. **Create and activate a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
```
3. **Install the required dependencies:**
```bash
pip install -r requirements.txt
```

### Dataset
The datasets we used are obtained from Kaggle and belong to The Movie Database(TMDb):
- tmdb_5000_credits.csv
- tmdb_5000_movies.csv

### TMDb API Setup
To run the project, you'll need a TMDb API key:
1. Sign up at TMDb and obtain an API key.
2. Replace the placeholder API key in app.py with your own.

## Running the Project

1. Start the Streamlit app:
```bash
streamlit run app.py
```
2. The app will open in your web browser. Type or select a movie,
   then click "Show recommendation" to see movie suggestions with posters.

## Known Issues
- **API Limitations:** TMDb API has a rate limit; excessive usage may result in temporary blocks.
- **Dataset Updates:** Ensure the dataset is updated to reflect the latest movies.

## Credits
- **The Movie Database (TMDb):** For the API and movie data.
- **Python Libraries:** Streamlit, Requests, Pandas, Scikit-learn, etc.
