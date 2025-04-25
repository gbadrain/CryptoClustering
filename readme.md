# CryptoClustering Project

## Overview
This project applies unsupervised machine learning techniques to analyze and cluster cryptocurrencies based on 24-hour and 7-day price changes. Using Python, Pandas, scikit-learn, and hvPlot, the project demonstrates data preprocessing, clustering analysis, and visualization skills. The results reveal patterns and trends in cryptocurrency behavior, showcasing expertise in data analytics and machine learning workflows.

## Project Goals
- Extract and preprocess cryptocurrency market data from a CSV file
- Use the elbow method to determine the optimal number of clusters (k) for K-means clustering
- Perform K-means clustering and visualize the results using scaled data
- Apply Principal Component Analysis (PCA) for dimensionality reduction to optimize clustering performance
- Compare clustering results with and without PCA to assess the impact of feature reduction
- Develop interactive visualizations for clear and actionable insights

## Repository Content

### 1. Jupyter Notebook
- **Crypto_Clustering.ipynb**:
  - Implements data preprocessing, clustering, and PCA logic
  - Visualizes clustering results using hvPlot
  - Analyzes and compares results from scaled and PCA-reduced datasets

### 2. Data Files
- **crypto_market_data.csv**:
  - Raw cryptocurrency market data containing 24-hour and 7-day price change percentages

### 3. Generated Outputs
- Scaled DataFrame and PCA-transformed DataFrame used for clustering analysis
- Interactive visualizations for K-means clustering and PCA comparison

## Instructions

### Part 1: Data Preparation
- Load the crypto_market_data.csv file into a Pandas DataFrame
- Generate summary statistics and visualize the data distribution

### Part 2: Data Scaling
- Normalize the dataset using StandardScaler from scikit-learn
- Create a scaled DataFrame with "coin_id" as the index

### Part 3: Clustering Analysis (Scaled Data)
- Use the elbow method to determine the optimal number of clusters (k)
- Implement K-means clustering with the optimal k value
- Add cluster labels to the scaled DataFrame
- Visualize clusters with hvPlot, using:
  - X-axis: price_change_percentage_24h
  - Y-axis: price_change_percentage_7d
  - Hover: coin_id

### Part 4: Dimensionality Reduction with PCA
- Apply PCA to reduce the dataset to three principal components
- Evaluate and record the explained variance of each component
- Create a PCA-transformed DataFrame for further analysis

### Part 5: Clustering Analysis (PCA Data)
- Repeat the elbow method and K-means clustering using the PCA-reduced dataset
- Visualize clusters with hvPlot, using:
  - X-axis: PC1
  - Y-axis: PC2
  - Hover: coin_id

### Part 6: Comparative Analysis
- Use composite plots to compare:
  - Elbow curves for scaled data vs PCA-reduced data
  - Clustering visualizations for scaled data vs PCA-reduced data
- Document the impact of dimensionality reduction on clustering performance

## Results
- **Optimal Clusters**: The elbow method identified the best value of k for both scaled and PCA-reduced data
- **Clustering Visualizations**: Clear and interactive visualizations of cryptocurrency clusters reveal market trends
- **Dimensionality Reduction**: PCA simplified the dataset while retaining key information, leading to similar clustering results with fewer features

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - Pandas: Data manipulation and analysis
  - scikit-learn: Machine learning algorithms for scaling, PCA, and K-means clustering
  - hvPlot: Interactive data visualizations
- **Tools**:
  - Jupyter Notebook: For developing and presenting the project

## Exploratory Insights
- Analyzed price change behavior to uncover distinct groups of cryptocurrencies
- Evaluated the impact of feature reduction on clustering accuracy and efficiency
- Enhanced understanding of clustering techniques and their practical applications

## Sources of Help
- Resources from University of Oregon Continuing and Professional Education Data Analytics Boot Camp
- Microsoft Copilot for problem-solving and guidance
- Python and scikit-learn documentation
- hvPlot documentation for interactive plotting
- Tutorials and guides on PCA and K-means clustering

## Acknowledgments
This project was created as part of a professional development challenge inspired by Module 19 curriculum. Special thanks to the developers of open-source tools and libraries that made this analysis possible.

## Contact
- **Name**: Gurpreet Singh Badrain
- **Role**: Market Research Analyst & Aspiring Data Analyst
- **GitHub**: https://github.com/gbadrain
- **Linkedin** : http://linkedin.com/in/gurpreet-badrain-b258a0219
- **Email**: gbadrain@gmail.com
