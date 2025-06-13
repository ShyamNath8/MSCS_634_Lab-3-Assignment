Lab 3: Clustering Analysis Using K-Means and K-Medoids

Purpose
The purpose of this lab is to explore unsupervised learning techniques, specifically clustering, using the Wine dataset from the `sklearn` library. The lab applies both K-Means and K-Medoids algorithms to group the dataset into clusters and evaluate their performance. This exercise is designed to develop practical understanding of clustering behavior, performance metrics (Silhouette Score and Adjusted Rand Index), and visualization of cluster structures.

Key Insights
-K-Means achieved higher Silhouette and ARI scores than K-Medoids, indicating more compact and accurate clusters relative to the original class labels.
-K-Medoids provided slightly less defined clusters but demonstrated robustness to outliers, since it selects actual data points as medoids.
-Visualizations using PCA showed that K-Means clusters were more symmetrical, while K-Medoids clusters had more irregular shapes due to their medoid constraint.

Challenges and Decisions
- A key challenge was installing the `scikit-learn-extra` package required for K-Medoids due to system dependency issues (Microsoft C++ Build Tools).
- To resolve this, alternative options such as using Google Colab or installing Visual C++ were considered.
- Choosing the correct evaluation metrics was also important. Silhouette Score was used to assess cluster cohesion, while Adjusted Rand Index allowed comparison against true labels.
- The number of clusters was set to 3 based on the known class distribution in the Wine dataset.

Conclusion
This lab demonstrated that while K-Means performs better for datasets with evenly distributed and spherical clusters, K-Medoids can be preferable when dealing with noisy data or when cluster centers need to be real data points.
