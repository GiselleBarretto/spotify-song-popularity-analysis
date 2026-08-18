# Spotify Song Popularity Analysis

## Project Overview

For this project, I wanted to explore a simple question:

**What characteristics are associated with popular Spotify songs?**

Using a dataset of over 170,000 songs from Kaggle, I analyzed audio features such as danceability, energy, acousticness, loudness, and tempo to understand how they relate to a song's popularity score.

The goal was not to predict popularity, but to identify patterns and understand how popular songs differ from the rest of the dataset.

---

## Dataset

The dataset used for this project was obtained from Kaggle:

Spotify Tracks Dataset by Yamac Eren Ay

Due to file size limitations, the raw dataset is not included in this repository.

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib

---

## Data Understanding and Cleaning

Before starting the analysis, I explored the dataset to understand its structure and quality.

I checked:

- Number of rows and columns
- Data types
- Missing values
- Duplicate records
- Summary statistics for numerical features

The dataset contained 170,653 songs and 19 columns. No missing values or exact duplicate rows were found.

I also investigated songs that appeared multiple times under the same artist. Since these records contained different values in other columns, they were retained as separate observations.

---

## Analysis

To better understand popularity, I first explored the distribution of popularity scores.

Some key observations:

- Average popularity score: 31.43
- Median popularity score: 33
- 75% of songs had a popularity score of 48 or lower

Based on this distribution, I classified songs with a popularity score of 70 or higher as **Popular** and compared them against the rest of the dataset.

I then performed:

- Correlation analysis
- Popular vs. Not Popular comparisons
- Data visualization

---

## Key Findings

- Only about 3% of songs had a popularity score of 70 or higher.
- Popular songs tend to be more energetic.
- Popular songs tend to be more danceable.
- Popular songs are generally louder.
- Acousticness showed the strongest negative relationship with popularity.
- Instrumental songs were less likely to be highly popular.
- Valence (how positive or happy a song sounds) showed little relationship with popularity.

---

## Conclusion

Based on this analysis, popular songs in this dataset tend to be more energetic, more danceable, less acoustic, and less instrumental than less popular songs.

While these characteristics are associated with popularity, they do not necessarily cause a song to become popular. Popularity can also be influenced by factors that are not included in the dataset, such as marketing, artist recognition, trends, and audience preferences.

This project helped me practice data cleaning, exploratory data analysis, correlation analysis, and data visualization using Python.
