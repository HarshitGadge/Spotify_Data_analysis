# Spotify Tracks: Exploratory Data Analysis

Exploratory analysis of about 587,000 Spotify tracks (releases from 1922 onward), covering popularity, audio features and how songs changed over time.

## Data

"Spotify Dataset 1921–2020, 600k+ Tracks" (Kaggle), `tracks.csv`: 586,672 tracks × 20 columns. It includes popularity (0–100), duration,
explicit flag, and audio features such as danceability, energy, loudness, speechiness, acousticness, instrumentalness, liveness, valence and tempo.

## What the notebook covers

- Data quality: 71 tracks with no name; all other fields complete
- The least popular tracks, and tracks with popularity above 90 (for example "Peaches" and "drivers license")
- Correlation heatmap of the audio features
- Scatter plots with regression lines: loudness vs energy, and popularity vs liveness (on a 0.4% random sample, for readability)
- Number of songs released per year, and average song duration by year

## Run it

The notebook was written on Kaggle and reads from `../input/spotify-datasets/tracks.csv`. To run it locally, download the CSV and update that path.

Tools: pandas, NumPy, matplotlib, seaborn.

Notebook: [`spotify-data-analysis.ipynb`](spotify-data-analysis.ipynb)
