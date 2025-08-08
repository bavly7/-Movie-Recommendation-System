# Movie Recommendation System
A recommendation system built on the MovieLens 100K dataset that implements user-based collaborative filtering, item-based collaborative filtering, and matrix factorization (SVD) approaches.

## Table of Contents
- [Features](#features)
- [Dataset](#dataset)
- [Algorithms Implemented](#algorithms-implemented)
- [Evaluation Metrics](#evaluation-metrics)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Features
- Three recommendation approaches:
  - User-based collaborative filtering
  - Item-based collaborative filtering
  - Matrix factorization (SVD)
- Leave-one-out evaluation methodology
- Precision@K metric calculation
- Example recommendation generation

## Dataset
The system uses the [MovieLens 100K dataset](https://grouplens.org/datasets/movielens/100k/) containing:
- 100,000 ratings (1-5) from 943 users on 1682 movies
- User demographic information
- Movie metadata (title, release date, genres)

## Algorithms Implemented

### 1. User-Based Collaborative Filtering
- Computes user similarity using mean-centered cosine similarity
- Predicts ratings based on ratings from similar users
- Generates top-K recommendations

### 2. Item-Based Collaborative Filtering
- Computes item similarity using mean-centered cosine similarity
- Predicts ratings based on similar items the user has rated
- Generates top-K recommendations

### 3. Matrix Factorization (SVD)
- Performs dimensionality reduction using Truncated SVD
- Captures latent factors in user-item interactions
- Reconstructs the rating matrix for predictions

## Evaluation Metrics
- **Precision@K**: Measures the percentage of held-out test items that appear in the top-K recommendations
- Leave-one-out evaluation: For each user, one rating is held out as test data

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/movie-recommendation-system.git
cd movie-recommendation-system
