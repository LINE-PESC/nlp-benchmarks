Stanford Sentiment Treebank
==========================


### Binary sentiment classification

> Lower is better

| Error rate |  Strategy | Reported by | Notes |
|------------|-----------|-------------|-------|

| 20.6%      | SVMs | Socher et al., 2013b | |
| 19.9%      | Word Vector averaging | Socher et al., 2013b | |
| 18.2%      | Naïve Bayes | Socher et al., 2013b | |
| 17.6%      | Recursive Neural Nets | Socher et al., 2013b | |
| 17.1%      | Matrix Vector-RNN | Socher et al., 2013b | |
| 16.9%      | Bi-gram Naïve Bayes | Socher et al., 2013b | |
| 14.6%      | Recursive Neural Tensor Network | Socher et al., 2013b | |
| 12.2%      | Paragraph2Vec | Le and Mikolov 2014 | Using a mixture of PV-DM and PV-DBOW |

### Fine-grained sentiment classification


#### References

- Le and Mikolov 2014: Distributed Representations of Sentences and Documents

- Socher et al., 2013a: Reasoning with neural tensor networks for knowledge base completion.

- Socher et al., 2013b : Recursive deep models for semantic compositionality over a sentiment treebank.