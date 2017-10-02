del.icio.us Custom Datasets
===================

Page reserved for tasks and articles using custom crawls of Delicious data.

Each article used a specific crawls of the website, so results may not be directly comparable.

### Tag Prediction 

| Precision@5 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|~0.31| SVM | Illig et al. 2011 | Global Approach |
|~0.30| LDATgg-100 | Hu 2010 | Global approach |

| Precision |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.4738 | MMSG (Multilabel Multiclass Sparse Gaussian Processes) | Song et al. 2011 | Global approach |
|0.4352 | PMM (Poisson Mixture Model) | Song et al. 2011 | Global approach |

| Recall@5 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|~0.7| SVM | Illig et al. 2011 | Global approach |
|~0.22| LDATgg-100 | Hu 2010 | Global approach |

| Recall |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.6616 | MMSG | Song et al. 2011 | Global approach |
|0.6231 | PMM | Song et al. 2011 | Global approach |

| F1@5 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|~0.44 | SVM | Illig et al. 2011 | Global approach|
|~0.20| LDATgg-100 | Hu 2010 | Global approach |

| F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.5423 | MMSG | Song et al. 2011 | Global approach |
|0.5277 | PMM | Song et al. 2011 | Global approach |

| NDCG@5 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|~0.35| LDATgg-100 | Hu 2010 | Global approach |

### References

- [Hu 2010: A Topic Modeling Approach to Social Tag Prediction](http://www.ieee-tcdl.org/Bulletin/v6n2/Hu/hu.html)

- Lipczak and Milios 2011: Efficient Tag Recommendation for Real-Life Data

- Illig et al. 2011: A Comparison of Content-Based Tag Recommendations in Folksonomy Systems

 - All posts between 2003-10-01 and 2004-08-26 have been used for the training dataset resulting in 4,236 users. For the set of test documents, we considered all 10,602 documents that occurred in posts between 2004-08-27 and the end of 2004-09-05. From these, we removed all 2,417 documents which also occurred in posts from the training set.

 - We limited  the set  to  only those documents with  at least  ten  tag assignments in the whole dataset

- Song et al. 2011: Automatic tag recommendation algorithms for social recommender systems

