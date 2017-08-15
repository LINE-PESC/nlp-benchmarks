StackExchange data
===================================

[Link to Data](https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data)

This dataset contains duplicate questions (data leaking). Scores achieved using that knowledge are naturally much higher.

### Tag Prediction

| Mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 0.471      | Fuzzy NNS | Hong and Feng 2013 | No leaked data. |
| 0.4149      | Co-occurrence and KNN | Hong and Feng 2013 | No leaked data. |
| 0.4123      | Co-occurrence and SVM | Hong and Feng 2013 | No leaked data. |
| 0.4100      | Keyword-tag co-occurrence | Hong and Feng 2013 | No leaked data. |

| Accuracy (1 tag per post)|  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 0.7105      | Fuzzy NNS | Hong and Feng 2013 | No leaked data. |
| 0.6370      | Co-occurrence and KNN | Hong and Feng 2013 | No leaked data. |
| 0.6315      | Keyword-tag co-occurrence | Hong and Feng 2013 | No leaked data. |
| 0.6170      | Co-occurrence and SVM | Hong and Feng 2013 | No leaked data. |

#### References

- Hong and Feng 2013: Keyword Extraction and Semantic Tag Prediction
