 # 🎵 Spotify Song Recommendation System

 This project is a song recommendation system build on a hybrid model of kmeans clustering and KNN,using a vast data set scraped from spotify, you get recommended a song based on various audio features and genre of songs.

 ## 📌 Features

- 🔍 Included **Fuzzy search** for partial song names.
- 🎯 **Feature-based** scaling for musical attributes like danceability, tempo, valence, etc.
- 🎶 **Genre-based** filtering and modeling.
- 🤝 **KNN-based** similarity recommendations.
- 📊 Visualizations for data understanding (e.g., PCA plots, heatmaps).

 ## 🛠️ Technologies Used
- **Python 3.10+**
- **Pandas, NumPy** — for data manipulation
- **Scikit-learn** — Kmeans and KNN models
- **Matplotlib**, Seaborn — visualizations
- **FuzzyWuzzy** — partial string matching
## 📁 Dataset

The dataset used contains a wide range of Spotify audio features for over 1 millions songs including:

- `danceability`, `energy`, `key`, `valence`, `tempo`, `duration_ms`
- `track_name`, `artist_name`

## 🚀 How It Works

1. **Data Preprocessing**
   - Clean and scale audio features.
   - Remove outliers using Z-score filtering.

2. **KMeans Clustering**
   - Cluster songs based on audio and genre features to find similar groups.

3. **Fuzzy Matching**
   - Used fuzzy matching to locate the closest song name from user input.

4. **KNN Modeling**
   - Use KNN to find the nearest neighbors in feature space and suggest similar songs.

## 🧪 Example

```python
recommend_similar_songs("Shape of You", k=5)
```

**Output:**
```
1. Dynamite - Acoustic
2. Watermelon Sugar
3. ... and 3 more similar tracks
```

## 📊 Visualizations

- **Pairplots and Correlation Heatmaps** to understand feature relationships
- **PCA / t-SNE plots** for feature space visualization (optional)

## 🔧 Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spotify-recommender.git
   cd spotify-recommender
   ```

2. Download the data set below
   
   [Dataset](https://www.kaggle.com/datasets/amitanshjoshi/spotify-1million-tracks)

4. Launch the notebook:
   ```bash
   jupyter notebook spotify.ipynb
   ```

## 🧠 Future Improvements

- Can add Spotify API integration for real-time dataa and user based personalisation.
- Build a web UI using **Streamlit** or **Gradio**.

## 📄 License

This project is licensed under the MIT License.
