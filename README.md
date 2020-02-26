# Keyphrase-extraction-for-research-articles

Model for extracting and ranking keyphrases from research articles using an unsupervised theme and position biased-PageRank
model. Part of Deep learning for NLP course in Fall 19 semester at the University of Illinois at Chicago.

### Requirements:
* Numpy
* [StanfordCoreNLP](https://stanfordnlp.github.io/CoreNLP/)
* [fastText embeddings](https://fasttext.cc/docs/en/english-vectors.html)
  > Embeddings used: wiki-news-300d-1M-subword.vec.zip. 1 million word vectors trained with subword infomation on Wikipedia 2017, UMBC webbase corpus and statmt.org news dataset (16B tokens). T. Mikolov, E. Grave, P. Bojanowski, C. Puhrsch, A. Joulin. Advances in Pre-Training Distributed Word Representations, LREC 2018
