# Movie Ratings Analysis with TMDB and MovieLens Datasets

Welcome to the **Movie Ratings Analysis** repository! This project focuses on analyzing movie ratings from two popular datasets: **TMDB 5000 Movies** and **MovieLens 100k**. The goal is to explore the distribution of movie ratings, compare datasets, and apply statistical methods to understand the data better.

---

## Project Overview

The project is divided into the following key steps:
1. **Data Loading & Exploration**:
   - Load and explore the TMDB and MovieLens datasets.
   - Analyze the distribution of movie ratings and other features like runtime, budget, and popularity.

2. **Data Visualization**:
   - Create visualizations (histograms, box plots, and cumulative distribution plots) to understand the data distribution and relationships.

3. **Statistical Analysis**:
   - Compare average ratings between datasets.
   - Apply statistical tests (e.g., z-test, t-test) to validate hypotheses about the data.

4. **Hypothesis Testing**:
   - Test whether the distribution of ratings is normal.
   - Compare ratings of specific movies (e.g., *Toy Story*, *Silence of the Lambs*, *Fantastic Mr. Fox*) using non-parametric tests.

---

## Datasets

### TMDB 5000 Movies
- **Source**: [Kaggle](https://www.kaggle.com/tmdb/tmdb-movie-metadata)
- **Features**:
  - `vote_average`: Average rating of the movie.
  - `vote_count`: Number of votes.
  - `budget`: Movie budget.
  - `popularity`: Popularity score.
  - `runtime`: Movie duration.

### MovieLens 100k
- **Source**: [MovieLens](https://grouplens.org/datasets/movielens/)
- **Features**:
  - `userId`: ID of the user who rated the movie.
  - `movieId`: ID of the movie.
  - `rating`: Rating given by the user (1 to 5).
  - `timestamp`: Timestamp of the rating.

---

## Key Findings

1. **Distribution of Ratings**:
   - Ratings in both datasets are not normally distributed.
   - Movies with fewer votes tend to have extreme average ratings (e.g., 0 or 10).

2. **Comparison of Datasets**:
   - The average rating in the MovieLens dataset is **3.43**, while in the TMDB dataset, it is **6.09**.
   - Movies with at least 10 votes show a more stable distribution of ratings.

3. **Statistical Tests**:
   - The z-test and t-test confirm that the average rating of *Toy Story* is significantly higher than the overall average in the MovieLens dataset.
   - Non-parametric tests (e.g., ranksums) were used to compare ratings between movies, as the data is not normally distributed.

4. **Visual Insights**:
   - Box plots and histograms reveal the spread and central tendency of ratings.
   - Cumulative distribution plots show how ratings accumulate over the dataset.

---

## Tools & Technologies

- **Python**: Primary programming language.
- **Pandas**: Data manipulation and analysis.
- **Seaborn & Matplotlib**: Data visualization.
- **Scikit-learn**: Statistical analysis and hypothesis testing.
- **Jupyter Notebook**: Interactive environment for code execution.

---
