This is a small `pyspark` notebook example analyzing the movie lens dataset to generate the count for each rating categories.

The notebook is available at 
[movie-lens-analysis.ipynb](movie-lens-analysis.ipynb) 

###  The dataset can be downloaded from 

```
wget http://files.grouplens.org/datasets/movielens/ml-100k.zip
unzip ml-100k.zip
```
### In the notebook, 2 ways are presented

* Using  `countByValue()` 

This is an action that returns a Python defaultdict, not RDD, so this should be used with caution - only for small dataset.


* Using`reduceByKey()`

This is a transformation which returns a RDD which then can be applied further transformations - this works well for very large dataset.


