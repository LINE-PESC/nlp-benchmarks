Stanford Sentiment Treebank (Socher et al., 2013)
==========================

Fully labeled parse trees (this is based upon Pang and Lee's 2005 "sentence-polarity dataset")

Every node in the trees are labelled according to the sentiment of the phrase it represents:

![labelled parse tree](http://i.imgur.com/cHp7pjT.png)

*Adapted from Socher et al 2013b*


### Binary sentiment classification

| Error rate |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 20.6%      | SVMs | Socher et al., 2013b |  |
| 19.9%      | Word Vector averaging | Socher et al., 2013b | |
| 18.2%      | Naïve Bayes | Socher et al., 2013b | |
| 17.6%      | Recursive Neural Nets | Socher et al., 2013b | |
| 17.1%      | Matrix Vector-RNN | Socher et al., 2013b | |
| 16.9%      | Bi-gram Naïve Bayes | Socher et al., 2013b | |
| 14.6%      | Recursive Neural Tensor Network | Socher et al., 2013b | |
| 12.2%      | Paragraph Vector | Le and Mikolov 2014 | Using a mixture of PV-DM and PV-DBOW |

### Fine-grained sentiment classification

| Error rate |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|
| 67.3%      | Word Vector averaging | Socher et al., 2013b |  |
| 59.3%      | SVMs | Socher et al., 2013b | |
| 59.0%      | Naïve Bayes | Socher et al., 2013b | |
| 58.1%      | Bi-gram Naïve Bayes | Socher et al., 2013b | |
| 56.8%      | Recursive Neural Net | Socher et al., 2013b | |
| 55.6%      | Matrix Vector-RNN | Socher et al., 2013b | |
| 54.3%      | Recursive Neural Tensor Network | Socher et al., 2013b | |
| 51.3%      | Paragraph Vector | Le and Mikolov 2014 | Using a mixture of PV-DM and PV-DBOW |

#### References

- Le and Mikolov 2014: Distributed Representations of Sentences and Documents

- Socher et al., 2013a: Reasoning with neural tensor networks for knowledge base completion.

- Socher et al., 2013b : Recursive deep models for semantic compositionality over a sentiment treebank.