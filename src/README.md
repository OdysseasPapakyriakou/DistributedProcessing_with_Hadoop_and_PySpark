# A project for the Data Intensive Systems course (INFOMDIS) for Utrecht University

By Odysseas Papakyriakou and Thanos Tsiamis

## Description
Given a heterogeneous dataset, the goal is to split the dataset into homogeneous parts. 
2 main things are needed:
* a **homogeneity function** that assesses how homogeneous the (part of the) dataset is
* a **method to split the dataset** into smaller homogeneous parts using the homogeneity function

For this project we developed our own homogeneity function and our own tree algorithm to split the dataset based on this function. The results are compared to a baseline solution, k-means clustering.

The data are processed in a distributed way with Hadoop using PySpark and Map-Reduce procedures.

For a more comprehensive description of the project the reader can refer to the report.
## How to run
Little to no configuration is needed as this project is built upon Google Colab's powerful servers.
If you are not familiar with Google Colab, a nice video can be found [here](https://www.youtube.com/watch?v=inN8seMm7UI).

Clicking the run button on the left hand side sequentially, for each cell, will allow you to run the platform.

The program is designed to compare the k-means algorithm with a tree algorithm we developed. There are three datasets on which the program has been tested, one of a small size (the Titanic dataset), one of a medium size (0.001% of the title_basics dataset from imdb), and one of a large size (0.01% of the title_basics dataset from imdb).
### Note
The user should run only one cell from section 2 of the Google Colab notebook: the cell that corresponds to the dataset they want. The cells are clearly labeled inside the notebook.
