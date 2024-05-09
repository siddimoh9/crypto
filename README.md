# Crypto Clustering Assignment README

## Introduction
This repository contains the submission for the Crypto Clustering assignment. In this assignment, we aim to cluster cryptocurrencies based on their market data using K-means clustering algorithm. The assignment involves several steps including data preparation, finding the optimal value for k, clustering using original data and PCA data, and visualizing and comparing the results.

## Instructions

### Renaming the File
1. Rename the `Crypto_Clustering_starter_code.ipynb` file as `Crypto_Clustering.ipynb`.

### Loading Data and Data Preparation
2. Load the `crypto_market_data.csv` into a DataFrame.
3. Get the summary statistics and plot the data to understand its structure before proceeding.
4. Use the `StandardScaler()` module from scikit-learn to normalize the data from the CSV file.
5. Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

### Finding the Best Value for k Using the Original Scaled DataFrame
6. Use the elbow method to find the best value for k.
    - Create a list with the number of k values from 1 to 11.
    - Compute the inertia with each possible value of k.
    - Plot a line chart with all the inertia values to identify the optimal value for k.

### Clustering Cryptocurrencies with K-means Using the Original Scaled Data
7. Initialize the K-means model with the best value for k.
8. Fit the K-means model using the original scaled DataFrame.
9. Predict the clusters to group the cryptocurrencies.
10. Create a scatter plot using hvPlot to visualize the clusters.

### Optimizing Clusters with Principal Component Analysis (PCA)
11. Perform PCA on the original scaled DataFrame to reduce features to three principal components.
12. Determine the explained variance of the principal components.
13. Create a new DataFrame with the PCA data.

### Finding the Best Value for k Using the PCA Data
14. Use the elbow method on the PCA data to find the best value for k.
15. Plot a line chart with inertia values computed with different values of k.
16. Compare the best k value obtained from PCA data with the one from the original data.

### Clustering Cryptocurrencies with K-means Using the PCA Data
17. Initialize the K-means model with the best value for k.
18. Fit the K-means model using the PCA data.
19. Predict the clusters to group the cryptocurrencies based on PCA data.
20. Visualize the clusters using a scatter plot.

### Visualizing and Comparing Results
21. Create composite plots to compare the elbow curves and cluster visualizations obtained from original data and PCA data.

## Requirements
For detailed requirements and grading rubric, refer to the assignment instructions provided.

## Deployment and Submission
- Clone this repository to your local machine.
- Add your files to the repository using the command line.
- Make sure to include appropriate commit messages.
- Submit a link to your GitHub repository for evaluation.

## Coding Conventions and Formatting
- Keep imports at the top of the file.
- Name functions and variables with lowercase characters and words separated by underscores.
- Follow DRY principles.
- Use concise logic and creative engineering where possible.

## Code Comments
Ensure your code is well-commented with concise, relevant notes for better understanding by other developers.

For any questions or concerns regarding this assignment, please reach out to the instructor or teaching assistant.
