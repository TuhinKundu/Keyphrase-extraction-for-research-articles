# Keyphrase-extraction-for-research-articles

Model for extracting and ranking keyphrases from research articles using an unsupervised theme and position biased-PageRank
graph. Part of Deep learning for NLP course in Fall 19 semester at the University of Illinois at Chicago.

### Requirements:
* Numpy
* Scipy
* stemming
* [StanfordCoreNLP](https://stanfordnlp.github.io/CoreNLP/)
* [fastText embeddings](https://fasttext.cc/docs/en/english-vectors.html)
  > Embeddings used: wiki-news-300d-1M-subword.vec.zip. 1 million word vectors trained with subword infomation on Wikipedia 2017, UMBC webbase corpus and statmt.org news dataset (16B tokens). T. Mikolov, E. Grave, P. Bojanowski, C. Puhrsch, A. Joulin. Advances in Pre-Training Distributed Word Representations, LREC 2018
  
### Dataset used
* Data from [KDD and WWW](https://sites.google.com/site/sujathadas/home/datasets) conferences
  > Sujatha Das Gollapalli and Cornelia Caragea. "Extracting Keyphrases from Research Papers using Citation Networks." In: Proceedings of the 28th American Association for Artificial Intelligence (AAAI 2014)
 
### Model

The goal of this project is to build a keyphrase extraction model that uses candidate keyphrases extracted from scholarly articles and rank them using a modified novel PageRank algorithm in an unsupervised graph model.

Keyphrase extraction enables faster processing by mapping multiword phrases to a document, that describe it the best. The task is important for building automated systems that are able to provide high level contextual and descriptive information about research articles which may be used for recommending articles to readers, identifying potential reviewers, highlighting research trends and mapping citations to articles. This project aims to generate candidate keyphrases from an embedding model and rank them using a modified PageRank algorithm while capturing information that would accurately represent or describe the paper. Some previous graph based models such as Key2vec and PositionRank, amongst other supervised and unsupervised keyphrase extraction models, have been used for background and ideation of the project.

### Credits

* PositionRank: Corina Florescu and Cornelia Caragea. "PositionRank: An Unsupervised Approach to Keyphrase Extraction from Scholarly Documents." In: Proceedings of the Annual Meeting of the Association for Computational Linguistics (ACL 2017)
* Key2vec: Debanjan Mahata, John Kuriakose, Rajiv Ratn Shah, Roger Zimmermann. "Key2Vec: Automatic Ranked Keyphrase Extraction from Scientific Articles using Phrase Embeddings." In Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 2 (Short Papers)
* Ideas for PositionRank implementation: https://github.com/ymym3412/position-rank
