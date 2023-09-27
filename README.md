# Movie Recommendation System

This repository contains code for building a movie recommendation system using four different approaches:

1. Popularity-based recommendation system
2. Content-based recommendation system
3. Collaborative filtering-based recommendation system
4. Hybrid recommendation system

## Table of Contents
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Dataset](#dataset)
- [Code Overview](#code-overview)
  - [Popularity-based Recommendation](#popularity-based-recommendation)
  - [Content-based Recommendation](#content-based-recommendation)
  - [Collaborative Filtering](#collaborative-filtering)
  - [Hybrid Recommendation](#hybrid-recommendation)
- [Usage](#usage)
- [License](#license)

## Introduction

A movie recommendation system is designed to suggest movies to users based on their preferences or behavior. In this repository, we implement four different recommendation approaches:

1. **Popularity-based Recommendation System**: This approach recommends movies based on their popularity among all users. It does not provide personalized recommendations but suggests movies that are generally popular.

2. **Content-based Recommendation System**: This approach recommends movies similar to the one the user has shown interest in. It uses movie metadata, such as genre and cast, to find similarities between movies.

3. **Collaborative Filtering-based Recommendation System**: Collaborative filtering considers the preferences and behavior of users. It suggests movies based on the preferences of users with similar tastes. We implement both user-user and item-item collaborative filtering.

4. **Hybrid Recommendation System**: The hybrid recommendation system combines multiple recommendation approaches to provide more accurate and diverse recommendations. In this case, we combine content-based and collaborative filtering methods.

## Requirements

To run the code in this repository, you need the following libraries installed:

- `numpy`
- `pandas`
- `seaborn`
- `matplotlib`
- `sklearn`
- `difflib`
- `requests`
- `tmdbv3api` (for content-based recommendation)

You can install these libraries using `pip`:

```bash
pip install numpy pandas seaborn matplotlib scikit-learn requests tmdbv3api
```

## Dataset

The code uses a movie dataset available in CSV format. You can replace it with your own dataset or use publicly available datasets. The dataset should contain information about movies, such as title, genre, release date, vote average, and vote count.

## Code Overview

### Popularity-based Recommendation

- Calculates the popularity of movies based on vote averages and vote counts.
- Implements a weighted average formula to recommend movies based on popularity.
- Provides a list of popular movies for all users.

### Content-based Recommendation

- Combines movie metadata (cast and crew, genre) into a single feature.
- Uses the CountVectorizer and cosine similarity to find similar movies.
- Provides recommendations based on user-specified movie titles.

### Collaborative Filtering

- Implements user-user and item-item collaborative filtering.
- Calculates user or item similarities using user ratings.
- Recommends movies based on user preferences or item similarities.
- Requires a separate ratings dataset.

### Hybrid Recommendation

- Combines content-based and collaborative filtering recommendations.
- Assigns weights to each recommendation approach and combines their scores to make hybrid recommendations.

## Usage

1. Clone this repository to your local machine.
2. Ensure you have the required libraries installed (see Requirements).
3. Replace the dataset with your own or use a publicly available dataset.
4. Run the individual recommendation scripts or the hybrid recommendation script as needed.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
