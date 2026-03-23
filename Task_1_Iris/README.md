 [cite_start]Task 1: Exploring and Visualizing a Simple Dataset 

 Objective
[cite_start]Understand how to read, summarize, and visualize a dataset[cite: 10, 11].

 Dataset
[cite_start]Iris Dataset.

Approach
 [cite_start]**Data Loading & Inspection:** Loaded the dataset using the `pandas` library[cite: 14]. [cite_start]Displayed dataset structure using `.shape`, `.columns`, and `.head()`.
  [cite_start]Basic Visualizations:** Used `matplotlib` and `seaborn` for visualizations  to create:
   [cite_start]A scatter plot to analyze relationships between variables[cite: 16, 17].
   [cite_start]A histogram to examine data distribution[cite: 16, 18].
  [cite_start]A box plot to detect outliers and spread of values[cite: 16, 19].
  Advanced EDA: Implemented a Seaborn Pairplot for multidimensional clustering and a Correlation Heatmap to mathematically prove feature relationships.

 Results and Insights
Basic Insights: The `setosa` species is distinctly isolated from the others based on its smaller petal and sepal dimensions. The box plot also successfully highlighted minor statistical outliers in the `setosa` category.
Advanced Insights: The Pairplot confirmed that while `versicolor` and `virginica` share some dimensional overlap, they can still be effectively clustered when evaluating multiple features simultaneously. The Correlation Heatmap mathematically proved a nearly perfect positive correlation between petal length and petal width.
