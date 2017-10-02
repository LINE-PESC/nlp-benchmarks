del.icio.us t-140 dataset (Zubiaga et al., 2009)
===================

[Link to dataset](http://nlp.uned.es/social-tagging/delicioust140/)

Dataset with resources and tags, only the top 140 most used tags are reported.

### Notes

- `tags2vec` and `EPTR` have been introduced by Kataria and Agarwal 2015

- `TransE` was introduced by Bordes et al. 2013

## Tag Prediction

| Precision@1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.5959| tags2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.5775| tags2vec representation (without content) with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.5595| doc2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.5362| doc2vec (content+tags) representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |

| Precision@10 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.4127| tags2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.3685| tags2vec representation (without content) with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.332843| doc2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.2835| doc2vec (content+tags) representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |

| Recall@1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.1084| tags2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.0920| tags2vec representation (without content) with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.0826| doc2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.0714| doc2vec (content+tags) representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |

| Recall@10 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.6355| tags2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.5782| tags2vec representation (without content) with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.5108| doc2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.4823| doc2vec (content+tags) representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |

| F1@1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.16541| tags2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.15702| tags2vec representation (without content) with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.1407| doc2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.1282| doc2vec (content+tags) representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |

| F1@10 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.4340| tags2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.4191| tags2vec representation (without content) with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.3451| doc2vec representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |
|0.3177| doc2vec (content+tags) representation with Sparse Gaussian Processes classification | Kataria and Agarwal 2015 | Global approach |

| MAP (Mean Average Precision) |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.36566| EPTR (Embedded Personalized Tag Recommendation) | Kataria and Agarwal 2015 | Local approach |
|0.31290| FM (Factorization Machine) | Kataria and Agarwal 2015 | Local approach |
|0.28038| PITF (Pairwise Interaction Tensor Factorization) | Kataria and Agarwal 2015 | Local approach |
|0.19791| TransE (Translation-based Embeddings) | Kataria and Agarwal 2015 | Local approach |

### References

- Zubiaga et al., 2009: Content-based Clustering for Tag Cloud Visualization

- Bordes et al. 2013: Translating Embeddings for Modeling Multi-relational Data

- [Kataria and Agarwal 2015: Distributed Representations for Content-Based and Personalized Tag Recommendation](http://ieeexplore.ieee.org/xpls/icp.jsp?arnumber=7395832)