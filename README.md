## Customer Clustering Project
[![](Image.jpg)](https://unsplash.com/photos/group-of-people-standing-in-front-of-food-stall-counter-66RxrYlPShI)

### Overview
This project applies **Unsupervised Machine Learning** techniques to a customer dataset to identify meaningful clusters. The goal is to segment customers based on their features, using some popular clustering algorithms such as **K-Means**, **DBSCAN** and **Gaussian Mixture Models (GMM)**. The clustering results are evaluated and visualized to extract actionable insights.

<br>

### Process Workflow
The project follows a structured approach for clustering:

1. **Data Cleaning:** <br>
Imported the dataset and handled missing values using *dropna()*.

2. **Data Visualization:** <br>
Explored the dataset through detailed visualizations (scatter plots, pair plots, bar charts, etc.) to understand feature relationships.

3. **Data Scaling:** <br>
Applied *MinMaxScaler* to normalize the dataset to the range [0, 1] for better performance with clustering algorithms.

4. **Clustering Algorithms:** <br>
Performed clustering using the following methods:

  - *K-Means Clustering:* Identified optimal clusters using Silhouette Score Analysis.
  - *DBSCAN:* Explored density-based clustering with parameter tuning (eps and min_samples).
  - *Gaussian Mixture Models (GMM):* Modeled clusters using probability distributions.

5. **Evaluation:** <br>
Used *Silhouette Score* to evaluate the clustering performance for all algorithms.

6. **Parameter Optimization:** <br>
Conducted parameter tuning for *K-Means*, *DBSCAN* and *GMM* to find the optimal number of clusters and density thresholds.

7. **Visualization:** <br>
Created various plots to interpret and compare clustering results:

  - Scatter plots with PCA reduction.
  - Heatmaps of cluster feature averages.
  - Barplot to illustrate the cluster's size.

<br>

### Results
After evaluation and parameter tuning:

  - **K-Means** provided the best clustering results with:
    - Optimal Number of Clusters: 2
    - Silhouette Score: 0.3906
  - **DBSCAN** struggled with the dataset, forming a single cluster and noise.
  - **GMM** gave reasonable results but was outperformed by K-Means in this case.

<br>

### Repository Contents

- **Data:** Contains the [Original Dataset](https://www.kaggle.com/datasets/mahnazarjmand/customer-segmentation) and you can see the cleaned dataset in notebook.

- **Notebook:** Jupyter notebook detailing the entire process, including data cleaning, visualization, clustering, and evaluation.

- **README.md:** Project documentation.

<br>

### How to Contribute
Contributions are welcome! If you'd like to improve the project or add new features:

1. **Fork the repository.**
2. **Create a new branch.**
3. **Make your changes and submit a pull request.**
