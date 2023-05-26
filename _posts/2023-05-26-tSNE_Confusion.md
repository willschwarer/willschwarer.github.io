# What is t-SNE

t-SNE while still important for this assignment, eludes my grasp on understanding it. I've made good progress in trying to and one really good resources has helped me out.

(https://distill.pub/2016/misread-tsne/?fbclid=IwAR2pmZ-s273cR5cvf20Uj8ega6cMO8UtEaEHyc8KzManwDlMnuGCnHMj7xI)

- The above website is summarsied below by ChatGPT better than I ever could.
- Hyperparameters matter: The hyperparameters of t-SNE, such as perplexity and the number of iterations, have a significant impact on the resulting plots. Experiment with different values of perplexity to balance the attention between local and global aspects of your data. It is recommended to analyze multiple plots with different perplexities to get the most accurate representation.
- Iterations until convergence: It's important to iterate until reaching a stable configuration. The number of iterations required for convergence may vary depending on the dataset, and there is no fixed number of steps that guarantees a stable result. Keep iterating until the plot no longer changes significantly.
- Cluster sizes in t-SNE plots: The sizes of clusters in t-SNE plots do not reflect the actual sizes of the clusters in the high-dimensional space. t-SNE adapts its notion of "distance" to regional density variations, expanding dense clusters and contracting sparse ones. As a result, it evens out cluster sizes. Therefore, you cannot rely on the sizes of clusters in t-SNE plots to determine the sizes of clusters in the original data.
- Distances between clusters: Distances between well-separated clusters in a t-SNE plot may not accurately represent the distances in the original high-dimensional space. While t-SNE can capture global geometry to some extent, there is no guarantee that the distances between clusters in the plot reflect their actual distances.
- Recognizing random noise: Be cautious when interpreting patterns in t-SNE plots, especially when dealing with random data. t-SNE can sometimes create clusters or structures in random data due to its non-linear nature. It's important to recognize when you are observing random noise rather than meaningful patterns.
- Multiple plots for topology: If you're interested in analyzing the topological properties of your data, you may need to examine multiple t-SNE plots with different perplexities. Different perplexity values can reveal different aspects of the topology, and combining the information from multiple plots can provide a more complete picture.
