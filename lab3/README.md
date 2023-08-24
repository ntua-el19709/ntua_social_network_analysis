# Link Prediction

In this exercise we use Machine Learning to predict the links of a network. More specificcaly, we will show 3 different methods of doing it (with increasing complexity):

## Method 1 - Similarity Based Prediction, without ML

In this method we decide whether a link exists if the metric Jaccard Coefficient is greater than a threshold. We repeat the process for different thresholds.

## Method 2 - Similarity Based Prediction, with ML

In this method we create a dataframe of links, and as features we use the metrics:

- Jaccard Coefficient
- Preferential Attachment
- Resource Allocation

Then we train a Random Forest classifier, and predict the links with that model.

## Method 3 - Random Walk Based Prediction, with ML

In this method we apply the algorithm Node2Vec to extract the features of the graph, and then we train a Random Forest classifier with this features. We predict the links with this model.

The exercise is implemented in Jupyter Notebook `SNA_lab3.ipynb` and the markdown text is in greek. The file used for the network is `out.dbpedia-similar`.
