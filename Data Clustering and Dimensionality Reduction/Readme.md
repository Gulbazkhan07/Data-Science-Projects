# Data clustering and dimensionality reduction
# Description of the project
Let's assume you want to design an environment to predict a class/category from a dataset based on specific features of that class. However, all the features are not strong enough or in other words features not that much variance/uniqueness across the classes. So, you have to design a clustering model.

# Solution


Inspection of the data and scale it to standardize.

<img src=''>
<img src=''>


Elbow method is used to deduce the optimal number of clusters for this dataset. By running iterations till 5 clusters, the elbow method displays an ELBOW at 3 clusters. The total number of unique classes in the dataset is also 3 so the results of the elbow method seem to be correct.

* Purity Score of K-means: 91.9
* PURITY OF EUCLIDEAN: 87.14
* PURITY OF MANHATTAN: 86.19
* PURITY OF CHEBYSHEV: 89.05
* PURITY OF MINKOWSKI: 87.14

# Answer
After computing all the distance metrices and performing clustering on these distance matrics, the results show that the chebyshev metric performs better than the rest of the distance metrics. Chebyshev ends up giving the purity score of 89, which is higher than the scores of all the other distance metrics. Therefore, chebyshev is the right distance metric for this type of dataset.

#QUESTION
Use selection criteria (ANOVA, Chi-squared) to select best three features and use them for K-Means clustering. Based on the purity score which feature set are you going to recommend and why?
# Answer


SELECTED FEATURES PURITY 87.62

<img src=''>
<img src=''>
The chisquare graph shows us the least important features and the anova graph shows us the scores for all the features. We can deduce from both the graphs that WIDTH is not an important feature in our dataset and should be dropped. Other than width, we came up with 4 different sets of features that we tested for Kmeans clustering and computed their purity scored.
Feature Set 4 with Std, Kurtosis and Min features has outperformed all the other feature sets by giving the highest purity for K means clustering.

# PCA with 99% & 89% Variance
Number of Features with 99% Variance: 4
Number of Features with 89% Variance: 2

<img src=''>
<img src=''>

We have used the feature matrix produced by PCA with 89% Variance and 99% Variance for K means clustering and compared their results in terms of purity scores. The putiry scores of 89 Variance with total 2 features seems to be significantly better than 99 Variance with 4 features. The 89 Variance gives a purity result of 91% whereas the purity result of 99 Variance is ~88%. Therefore, for this particular dataset, PCA with 89 Variance is a better option.




