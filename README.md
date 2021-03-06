# Stat663FinalProject-Matt_Yamac
Final Project for Sta 663  by Matt Welch and Yamac Isik.

# Bayesian Hierarchical Clustering

An hiearchichal clustering method that uses a prior distribution to decide which clusters to form.This algorithm uses a tree node structure class to build the resulting tree coming the clustering process. For more information on the algorithm see : http://www2.stat.duke.edu/~kheller/bhcnew.pdf

Package is downloadable and installable via pip

$ pip install bayescluster

or

$ pip install --index-url https://test.pypi.org/simple/ bayescluster

# Using the Package

---Cluster Function---

```python
  >>> from bayes_cluster import cluster,mesures
  >>> cluster.clust()
  >>> clust(X,alpha,kappa0,v0,mu0,eta0,k)
   ```
@X: Features of the data set, must be a numpy array

@alpha:parameter to be set based on the number of clusters

@kappa0,v0,mu0,eta0 : See the report for explanations

@k: number of clusters to be determined

Returns a numpy array y, and a tree node structure tree

@y:numpy array giving the classifications of each observations

@tree: A tree structure which uses nodes, can be further used in the impurity calculations

 ---Impurity Measurement---
 
```python
  >>> from bayes_cluster import cluster,mesures
  >>>measures.impurity(tree,yhat,y,n=500)
  ```

@tree: tree node given by the algorithm

@yhat: predictions of the classifications

@y:original classification coming from the data set

@n=number of iterations







