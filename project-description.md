# Project Description | Vehicle Silhouettes
 
## Intro

Welcome to the project section! Here we will provide all of the details you need to understand the business-problem you are going to tackle. Let’s begin with the dataset!

## Data Description

The data that you’ll work with in this project contains features extracted from the silhouette of vehicles in different angles. In other words, all of the features that you are going to work with are geometric features extracted from the silhouette. They all are numeric in nature.

Features from the silhouette in the dataset are for the three vehicles. Here the are:

- a bus (which is a double decker bus)
- a van (which is a Cheverolet van)
- a car (either Saab 9000 or Opel Manta)

This particular combination of vehicles was chosen with the expectation that the bus, van and either one of the cars would be readily distinguishable, but it would be more difficult to distinguish between the cars.

The dataset is available for downloading [here](vehicle-silhouettes.csv). Let’s briefly discuss what kind of columns this dataset has:

- the `class` column contains vehicle models. As we discussed previously, there may be 3 values there: `bus`, `van` or `car`.
- the rest of the columns are numerical columns that describe the silhouette. Don’t worry if you don’t fully understand the rationale behind these columns. Treat them as some numbers that can tell you something about a silhouette of a particular vehicle. Here are these columns:

   - `compactness`
   - `circularity`
   - `distance_circularity`
   - `radius_ratio`
   - `pr.axis_aspect_ratio`
   - `max.length_aspect_ratio`
   - `scatter_ratio`
   - `elongatedness`
   - `pr.axis_rectangularity`
   - `max.length_rectangularity`
   - `scaled_variance`
   - `scaled_variance.1`
   - `scaled_radius_of_gyration`
   - `scaled_radius_of_gyration.1`
   - `skewness_about`
   - `skewness_about.1`
   - `skewness_about.2`
   - `hollows_ratio`

## Problem Description

A chain of car repair shops called **“Prospect Auto”** asked you for models that can differentiate vehicles based on their silhouettes. The goal is to explore both supervised and unsupervised approaches to see which provides the most effective solution.

## Steps in the Project 

- Import all required libraries, upload the dataset, and read it in.
- Conduct Exploratory Data Analysis (EDA) to understand the data visually and numerically.
- Prepare the dataset (cleaning, normalization/standardization, splitting into training and testing subsets).

### Supervised Learning Approach

- Train classification models using labeled data.
- Evaluate performance with metrics such as accuracy, precision, recall, and F1-score.
- Conclude whether the supervised model is suitable for deployment.

### Unsupervised Learning Approach

- Apply dimensionality reduction (e.g., PCA) to reduce features while preserving variance.
- Train clustering models (e.g., k-means, hierarchical clustering).
- Evaluate clustering quality using metrics such as silhouette score and inertia.
- Conclude whether unsupervised clustering provides meaningful groupings.

### Comparison

- Compare supervised and unsupervised results.
- Conclude which approach works best for Prospect Auto’s classification needs.
