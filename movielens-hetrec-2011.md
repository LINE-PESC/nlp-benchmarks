movielens-hetrec-2011
========================

[Link to dataset](https://grouplens.org/datasets/hetrec-2011/)

## Tag prediction/recommendation

| F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 0.243| FasTag (similar to Item-based CF) + blsC | Gueye et al. 2014 | Personalized |
| 0.179| FasTag | Gueye et al. 2014 | Personalized |
| 0.170 | argmax(t) of p(t|u,i) | Gueye et al. 2014 | Personalized |
| 0.167 | FolkRank | Gueye et al. 2014 | Personalized |
|0.14825 | STRec (Similar to Item-based CF) | Gueye et al. 2013 | Personalized |


### References

- Gueye et al. 2013: STRec: An Improved Graph-based Tag Recommender

- Gueye et al. 2014: A Social and Popularity-Based Tag Recommender