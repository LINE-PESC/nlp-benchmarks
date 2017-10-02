Bibsonomy Dataset (2009 ECML PKDD Challenge)
=========================

[https://www.kde.cs.uni-kassel.de/ws/dc09/](https://www.kde.cs.uni-kassel.de/ws/dc09/)

This dataset has tag-assignment information for resources hosted on BibSonomy.

The resources are divided into two parts.

### Part 1): bookmarks

Information on bookmarks made by users on the website. Attributes include:

- url
- description
- extended description
- date added

### Part 2): bibtex (Articles)

Normal bibtex fields, such as:

- title
- abstract
- description
- authors

### Dataset statistics:

- \# Bookmarks (full dataset): 235,328
- \# Articles (full dataset): 143,050
- \# Tags (full dataset): 93,756
- \# Bookmarks (post-core 2): 14,443
- \# Articles (post-core 2): 7,946
- \# Tags (post-core 2): 13,276


### Tag Prediction/Recommendation NOT on Post-core 2 (Task 1 of ECML PKDD)

> I.e., only for resources,users and tags which have LESS than 2 assignments

| F1 (micro-averaged) / Mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.18740| Extracted features from resource titles and urls | Lipczak et al., 2009 | |
|0.18001| Extracted tags from titles, web pages (in the case of urls) and previous tags given to that resource. Then each of these recommendations is weighted and a final prediction is given. | Mrosek et al., 2009 | |
|0.17975| Extract tag suggestions from the resource texts, from tags previously assigned to that resource and from tags given by that user to other resources, then learns weights to combine these into a final recommendation. | Ju and Hwang 2009 | Personalized Predictions |
|0.14151| CF-based | Zhang et al 2009 |  |
|0.1408 | Keywords and Association Rules | Wang et al. 2009 | |
| 0.11886 | FDT (Feature-Driven Tagging) Similar to Feature Engineering | Si et al .2009 | Not Personalized |


### Tag Prediction/Recommendation on Post-core 2 (Task 2 of ECML PKDD)

> These are all @5

| F1 (micro-averaged) / Mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 0.35594 | PITF (Pairwise Interaction Tensor Factorization) | Rendle and Schmidt-Thieme 2009 | Personalized |
| ~0.35 | FM (Factorization Machine) | Rendle 2010 | Personalized |
| 0.34791 | FasTag + Blsc (a method to tune the number of recommended tags) | Gueye et al. 2014 | Personalized|
| 0.33185 | Relational Classification | Marinho et al. 2009 | |
| 0.32461 |  Content-based| Lipczak et al. 2009 |  |
| 0.32230 | Content-based | Zhang et al. 20009 | |
| 0.3154 | SimRate | Zhang et al. 2014 | Personalized|
| 0.315| FasTag (Similar to User-Based CF) | Gueye et al 2014 | Personalized|
| 0.308 | maxarg(t) of p(t|u,i) | Gueye et al. 2014 | Personalized|
| 0.3075 | Diffusion Rank | Si et al. 2009 | Personalized|
| 0.305 | STRec | Gueye et al .2014 | Personalized |
| 0.3018 | FDT  (Feature-Driven Tagging) Similar to Feature Engineering | Si et al. 2014 | Personalized |
| 0.288 | PopRes | Rendle and Schmidt-Thieme 2009 | Not Personalized |
| 0.285 | FolkRank | Gueye et al. 2014 | Personalized |
| 0.2536 | PopRes (Most popular tags by resource)| Zhang et al. 2014 | Not personalized |
| 0.2382 | Cosine on Content features | Zhang et al. 2014 | Not personalized |

### Tag Prediction/Recommendation on Post-core 2 (Results on Training set (via CV))

| F1 (micro-averaged) / Mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 0.4110 | PopRes,PopUser | Si et al. 2014 | Personalized, bibtex only |
| 0.3959 | Content-based kNN | Si et al. 2014 | Personalized, bibtex only |
| 0.351 | PopRes | Rendle and Schmidt-Thieme 2009 | Not personalized |
| 0.3018 | FDT | Si et al. 2009 | Not personalized, bookmark only | 
| 0.2646 | Search-based KNN (Mishne 2006) | Si et al. 2009 |  Not-personalized, bookmark only |
| 0.2537 | Search-based KNN (Mishne 2006) | Si et al. 2009 |  Not-personalized, bibtex only |
| 0.2478 | FDT | Si et al. 2014 | Not personalized, bibtex only |


### References

- Lipczak et al. 2009: Tag Sources for Recommendation in Collaborative Tagging Systems

- Mrosek et al. 2009: Content- and Graph-based Tag Recommendation: Two Variations

- Ju and Hwang 2009: A Weighting Scheme for Tag Recommendation in Social Bookmarking Systems

- Si et al. 2009: Content-based and Graph-based Tag Suggestion

- Zhang et al. 2009: A Collaborative Filtering Tag Recommendation System based on Graph

- Gueye et al. 2014: A Social and Popularity-Based Tag Recommender 

- Zhang et al. 2014: Hybrid Personalized Tag Recommendation Algorithm Design and Evaluation

