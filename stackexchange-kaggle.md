StackExchange data (Kaggle)
===================================

[Link to Data](https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data)

Most of the data in the test set is also in the training set so if you take that information into account (data leaking), you get artificially high f1 scores.

### Tag Prediction

| Mean-F1 |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 0.77326      | Fuzzy NNS | Hong and Feng 2013 | Scored by Kaggle. Using leaked information. |
| 0.71132 | OvR SVM (Vowpal Wabbit) | Parikh 2013 | Scored by Kaggle. Using leaked information. Used only 500 top tags. Used some sort of variance-based feature selection. |
| 0.59 | OvR Linear SVM | González et al. 2015 | Probably scored by Kaggle. Used SVM Feature Selection. Their results are too high for them to have used original training data into train/test sets. They probably ran the test cases without realizing that they were in the training set too. | 
| 0.471      | Fuzzy NNS | Hong and Feng 2013 | Split original training data into train/test sets |
| 0.4149      | Co-occurrence and KNN | Hong and Feng 2013 | Split original training data into train/test sets |
| 0.4123      | Co-occurrence and SVM | Hong and Feng 2013 | Split original training data into train/test sets |
| 0.4100      | Keyword-tag co-occurrence | Hong and Feng 2013 | Split original training data into train/test sets |
| 0.41        | OvR Linear SVM | Schuster et al 2013 | Split original training data into train/test sets |
| 0.39 | OvR Naïve Bayes | González et al. 2015 | Probably scored by Kaggle. Used SVM Feature Selection. Their results are too high for them to have used original training data into train/test sets. They probably ran the test cases without realizing that they were in the training set too. |
| 0.39 (the guy said almost 40%) | Bagging and Linear SVM | Lucido 2013 | Scored by Kaggle. This guy probably didn't realize there were duplicates. |
| 0.3648 | OvR SVM (Vowpal Wabbit) | Parikh 2013 | No leaking. Used only 500 top tags. Used some sort of variance-based feature selection. | 

| Accuracy (1 tag per post)|  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 0.7105      | Fuzzy NNS | Hong and Feng 2013 | Split original training data into train/test sets |
| 0.6370      | Co-occurrence and KNN | Hong and Feng 2013 | Split original training data into train/test sets |
| 0.6315      | Keyword-tag co-occurrence | Hong and Feng 2013 | Split original training data into train/test sets |
| 0.6170      | Co-occurrence and SVM | Hong and Feng 2013 | Split original training data into train/test sets |

#### References

- Hong and Feng 2013: Keyword Extraction and Semantic Tag Prediction

- Lucido 2013: Large-scale Social Tag Prediction

- Parikh 2013: Identifying Tags from Millions of text Questions

- Schuster et al 2013: Predicting Tags for Stackoverflow Questions

- González et al 2015: Multi-class Multi-tag Classifier System for StackOverflow Questions