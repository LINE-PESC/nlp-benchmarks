Bibsonomy Dataset (2009 ECML PKDD Challenge)
=========================

[https://www.kde.cs.uni-kassel.de/ws/dc09/](https://www.kde.cs.uni-kassel.de/ws/dc09/)


### Task 1: Content-Based Tag Recommendations 

| mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
|0.18740| Extracted features from resource titles and urls | Lipczak et al., 2009 | Personalized Predictions |
|0.18001| Extracted tags from titles, web pages (in the case of urls) and previous tags given to that resource. Then each of these recommendations is weighted and a final prediction is given. | Mrosek et al., 2009 | Personalized Predictions |
|0.19975| Extract tag suggestions from the resource texts, from tags previously assigned to that resource and from tags given by that user to other resources, then learns weights to combine these into a final recommendation. | Sanghun et al., 2009 | Personalized Predictions |

### Task 2: Graph-Based Recommendations

| mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|

### Task 3: Online Tag Recommendations

| mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|

### References

- Lipczak et al., 2009: Tag Sources for Recommendation in Collaborative Tagging Systems

- Mrosek et al., 2009: Content- and Graph-based Tag Recommendation: Two Variations

- Sanghun et al., 2009: A Weighting Scheme for Tag Recommendation in Social Bookmarking Systems