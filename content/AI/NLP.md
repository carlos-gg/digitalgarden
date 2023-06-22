---
title: "Natural Language Processing (NLP)"
---

> A Computer Science field connected to Artificial Intelligence and Computational Linguistics which focuses on interactions between computers and human language and a machine’s ability to understand, or mimic the understanding of human language

> See:
> - [[AI/Foundation models]]
> - [[AI/Deep learning/Multimodal learning]]

## Resources
- https://en.wikipedia.org/wiki/Natural_language_processing
- NLP is a branch of data science that consists of systematic processes for analyzing, understanding, and deriving information from the text data in a smart and efficient manner. By utilizing NLP and its components, one can organize the massive chunks of text data, perform numerous automated tasks and solve a wide range of problems such as – automatic summarization, machine translation, named entity recognition, relationship extraction, sentiment analysis, speech recognition, and topic segmentation etc.
- https://github.com/keon/awesome-nlp
- [The most important NLP highlights of 2018](https://github.com/omarsar/nlp_highlights)
- [NLP - Udemy ML](https://github.com/jmportilla/Udemy---Machine-Learning/blob/master/NLP%20(Natural%20Language%20Processing).ipynb)
- https://www.analyticsvidhya.com/blog/2017/01/ultimate-guide-to-understand-implement-natural-language-processing-codes-in-python/
- https://www.datascience.com/blog/introduction-to-natural-language-processing-lexical-units-learn-data-science-tutorials
- https://github.com/BotCube/awesome-bots
- http://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html
- [Hidden Markov model](https://en.wikipedia.org/wiki/Hidden_Markov_model) 
- [Speech recognition](https://www.wikiwand.com/en/Speech_recognition)

### Text preparation
- http://nitin-panwar.github.io/Text-prepration-before-Sentiment-analysis/
	- Removing numbers
	- Removing Urls and Links
	- Removing stopwords
	- Stemming words
	- Suffix-dropping algorithms
	- Lemmatisation algorithms
	- n-gram analysis
	- Removing punctuation
	- Stripping whitespace
	- Checking for impure characters
- http://thinknook.com/10-ways-to-improve-your-classification-algorithm-performance-2013-01-21/

### Feature engineering
- https://www.geeksforgeeks.org/feature-extraction-techniques-nlp/
- https://www.analyticsvidhya.com/blog/2017/01/ultimate-guide-to-understand-implement-natural-language-processing-codes-in-python/

#### Bag of words
- A commonly used model in methods of Text Classification. As part of the BOW model, a piece of text (sentence or a document) is represented as a bag or multiset of words, disregarding grammar and even word order and the frequency or occurrence of each word is used as a feature for training a classifier.
- BoW is different from Word2vec, which we’ll cover next. The main difference is that Word2vec produces one vector per word, whereas BoW produces one number (a wordcount). Word2vec is great for digging into documents and identifying content and subsets of content. Its vectors represent each word’s context, the ngrams of which it is a part. BoW is good for classifying documents as a whole.

#### tf–idf 
- [tf-idf](https://en.wikipedia.org/wiki/Tf%E2%80%93idf)
- Term Frequency-Inverse Document Frequency
- tf–idf, is a numerical statistic that is intended to reflect how important a word is to a document in a collection or corpus.
-  The tf-idf value increases proportionally to the number of times a word appears in the document, but is often offset by the frequency of the word in the corpus, which helps to adjust for the fact that some words appear more frequently in general.
- https://deeplearning4j.org/bagofwords-tf-idf
- http://www.tfidf.com/
- http://scikit-learn.org/stable/auto_examples/text/document_clustering.html#sphx-glr-auto-examples-text-document-clustering-py

#### Word embeddings
- Word embedding is the modern way of representing words as vectors. The aim of word embedding is to redefine the high dimensional word features into low dimensional feature vectors by preserving the contextual similarity in the corpus. They are widely used in deep learning models such as Convolutional Neural Networks and Recurrent Neural Networks.
- #PAPER [Word2Vec: Distributed Representations of Words and Phrases and their Compositionality (Mikolov 2013)](https://arxiv.org/abs/1310.4546)
	-  https://papers.nips.cc/paper/5021-distributed-representations-of-words-and-phrases-and-their-compositionality.pdf
	- Skip-gram model with negative sampling
	- https://code.google.com/archive/p/word2vec/
	- [Paper explained](https://www.youtube.com/watch?v=yexR53My2O4)
	- http://p.migdal.pl/2017/01/06/king-man-woman-queen-why.html
	- http://www.deeplearningweekly.com/blog/demystifying-word2vec
	- http://multithreaded.stitchfix.com/blog/2017/10/18/stop-using-word2vec/
- #PAPER [Distributed representations of sentences and documents (Le 2014)](https://dl.acm.org/doi/10.5555/3044805.3045025)
	- https://medium.com/scaleabout/a-gentle-introduction-to-doc2vec-db3e8c0cce5e
- #PAPER [GloVe: Global Vectors for Word Representation (Pennington 2014)](https://aclanthology.org/D14-1162/)
	- [Glove](http://nlp.stanford.edu/projects/glove/)
	 - GloVe is an unsupervised learning algorithm for obtaining vector representations for words. Training is performed on aggregated global word-word co-occurrence statistics from a corpus, and the resulting representations showcase interesting linear substructures of the word vector space.
 - #PAPER [sense2vec - A Fast and Accurate Method for Word Sense Disambiguation In Neural Word Embeddings (Trask 2015)](https://arxiv.org/abs/1511.06388)
	 - [Sense2vec](https://explosion.ai/blog/sense2vec-with-spacy)
 - #PAPER [Enriching Word Vectors with Subword Information (Bojanowski 2017)](https://arxiv.org/abs/1607.04606)


### Semantics
#### Distributional semantics
- General recipe:
	- form a word-context matrix of counts (data)
	- perform dimensionality reduction ([[AI/Math and Statistics/SVD]]) for generalization
- For LSA the context is the document where the word appears.
- For word2vec the context is just a work, nearby words (in some window)  in a document.
- [Latent semantic analysis](https://en.wikipedia.org/wiki/Latent_semantic_analysis)
	- The process of analyzing relationships between a set of documents and the terms they contain. Accomplished by producing a set of concepts related to the documents and terms. LSA assumes that words that are close in meaning will occur in similar pieces of text.
	- Latent semantic analysis (LSA) is a technique in natural language processing, in particular distributional semantics, of analyzing relationships between a set of documents and the terms they contain by producing a set of concepts related to the documents and terms. 
	- LSA assumes that words that are close in meaning will occur in similar pieces of text. A matrix containing word counts per paragraph (rows represent unique words and columns represent each paragraph) is constructed from a large piece of text and SVD is used to reduce the number of rows while preserving the similarity structure among columns. Words are then compared by taking the cosine of the angle between the two vectors (or the dot product between the normalizations of the two vectors) formed by any two rows. Values close to 1 represent very similar words while values close to 0 represent very dissimilar words.
	- http://mccormickml.com/2016/03/25/lsa-for-text-classification-tutorial/
	- https://github.com/chrisjmccormick/LSA_Classification/blob/master/runClassification_LSA.py
	- http://stackoverflow.com/questions/30590881/python-lsa-with-sklearn

#### Topic Modelling
- https://en.wikipedia.org/wiki/Topic_model
- [Latent Dirichlet Allocation](https://es.wikipedia.org/wiki/Latent_Dirichlet_Allocation)
	- A common topic modeling technique, LDA is based on the premise that each document or piece of text is a mixture of a small number of topics and that each word in a document is attributable to one of the topics.
	- http://engineering.flipboard.com/2017/02/storyclustering
	- http://scikit-learn.org/stable/modules/generated/sklearn.decomposition.LatentDirichletAllocation.html
	- http://ahmedbesbes.com/how-to-mine-newsfeed-data-and-extract-interactive-insights-in-python.html

#### Neural semantic parsing
- #PAPER [Neural Semantic Parsing (Jia & Liang 2016)](https://www.aclweb.org/anthology/P18-5006/)

#### Explicit semantic analysis
- https://en.wikipedia.org/wiki/Explicit_semantic_analysis
- In NLP and information retrieval, explicit semantic analysis (ESA) is a vectorial representation of text (individual words or entire documents) that uses a document corpus as a knowledge base. Specifically, in ESA, a word is represented as a column vector in the tf–idf matrix of the text corpus and a document (string of words) is represented as the centroid of the vectors representing its words. Typically, the text corpus is English Wikipedia, though other corpora including the Open Directory Project have been used.
- Used in Information Retrieval, Document Classification and Semantic Relatedness calculation (i.e. how similar in meaning two words or pieces of text are to each other), ESA is the process of understanding the meaning of a piece text, as a combination of the concepts found in that text.
- Corpus or Corpora. A usually large collection of documents that can be used to infer and validate linguistic rules, as well as to do statistical analysis and hypothesis testing.

### Sentiment analysis
- https://en.wikipedia.org/wiki/Sentiment_analysis
- The use of NLP techniques to extract subjective information from a piece of text. i.e. whether an author is being subjective or objective or even positive or negative
- http://varianceexplained.org/r/trump-tweets/
- http://blog.aylien.com/sentiment-analysis-of-2-2-million-tweets-from-super-bowl-51/

### Deep learning-based
- [Modern Deep Learning Techniques Applied to Natural Language Processing](https://nlpoverview.com/)
- https://github.com/brianspiering/awesome-dl4nlp
- [Deep Learning in NLP](https://veredshwartz.blogspot.com/2018/08/deep-learning-in-nlp.html#)
- https://softwaremill.com/deep-learning-for-nlp/
- http://blog.aylien.com/modeling-documents-generative-adversarial-networks/
- [New AI classifier for indicating AI-written text](https://openai.com/blog/new-ai-classifier-for-indicating-ai-written-text)

#### CNN-based 
See [[AI/Deep learning/CNNs]]
- [Convolutional Neural Network for Sentence Classification](https://cnvrg.io/cnn-sentence-classification/)
- http://www.kdnuggets.com/2017/05/deep-learning-extract-knowledge-job-descriptions.html
- [How to read: Character level deep learning](https://offbit.github.io/how-to-read/)
- #PAPER [Connectionist Temporal Classification (Hannun 2017)](https://distill.pub/2017/ctc/)

#### RNN-based 
See [[AI/Deep learning/RNNs]]
- [RNN for NLP](https://adeshpande3.github.io/adeshpande3.github.io/Deep-Learning-Research-Review-Week-3-Natural-Language-Processing)
- http://www.abigailsee.com/2017/04/16/taming-rnns-for-better-summarization.html
- #PAPER [RRA: Recurrent Residual Attention for Sequence Learning (Wang 2017)](https://arxiv.org/abs/1709.03714)

#### Seq2seq
- #PAPER [Sequence to Sequence Learning with Neural Networks (Sustkever 2014)](https://arxiv.org/abs/1409.3215)
- Sequence-to-sequence models are deep learning models that have achieved a lot of success in tasks like machine translation, text summarization, and image captioning. Google Translate started using such a model in production in late 2016. These models are explained in the two pioneering papers (Sutskever et al., 2014, Cho et al., 2014).
- A sequence-to-sequence model is a model that takes a sequence of items (words, letters, features of an images…etc) and outputs another sequence of items. 
- Under the hood, the model is composed of an encoder and a decoder. The encoder processes each item in the input sequence, it compiles the information it captures into a vector (called the context). After processing the entire input sequence, the encoder sends the context over to the decoder, which begins producing the output sequence item by item.
- The context is a vector (an array of numbers, basically) in the case of machine translation. The encoder and decoder tend to both be recurrent neural networks.
- https://jalammar.github.io/visualizing-neural-machine-translation-mechanics-of-seq2seq-models-with-attention/
- [Encoder-Decoder LSTMs for sequence-to-sequence prediction](https://machinelearningmastery.com/encoder-decoder-long-short-term-memory-networks/)

#### Google Neural Machine Translation
- https://en.wikipedia.org/wiki/Google_Neural_Machine_Translation
- #PAPER [Zero-shot translation](https://arxiv.org/abs/1611.04558)
- Google Neural Machine Translation (GNMT) is a neural machine translation (NMT) system developed by Google and introduced in November 2016, that uses an artificial neural network to increase fluency and accuracy in Google Translate.
- https://research.googleblog.com/2016/11/zero-shot-translation-with-googles.html   

#### Transformer-based
See "For NLP" section in [[AI/Deep learning/Transformers]]

## Books
- #BOOK [Natural Language Processing with Python (Bird, 2013 OREILLY)](http://www.datascienceassn.org/sites/default/files/Natural%20Language%20Processing%20with%20Python.pdf)
- #BOOK [Mastering NLP with Python (Chopra, 2016 PACKT)](https://www.packtpub.com/big-data-and-business-intelligence/mastering-natural-language-processing-python)
	- https://github.com/PacktPublishing/Mastering-Natural-Language-Processing-with-Python
- #BOOK [An Introduction to Information Retrieval (Manning 2009, CAMBRIDGE)](https://nlp.stanford.edu/IR-book/)
- #BOOK [Text mining with R (Silge, 2020 OREILLY)](https://tidytextmining.com/)

## Courses
- #COURSE [Neural networks for NLP](http://phontron.com/class/nn4nlp2017/#) (Carnegie Mellon)
	- https://github.com/neubig/nn4nlp-code
	- https://www.youtube.com/user/neubig/videos
- #COURSE [NLP (Standford 15)](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1162/)
- #COURSE [NLP with Deep Learning  (Standford 16,17)](http://web.stanford.edu/class/cs224n/)
- #COURSE [Natural Language Understanding (Standford 16)](http://web.stanford.edu/class/cs224u/)
- #COURSE [Deep Learning for NLP (Oxford/Deepmind 17)](https://www.cs.ox.ac.uk/teaching/courses/2016-2017/dl/)
	- https://github.com/oxford-cs-deepnlp-2017
	- https://github.com/oxford-cs-deepnlp-2017/lectures
	- https://www.youtube.com/playlist?list=PL613dYIGMXoZBtZhbyiBqb0QtgK6oJbpm
- #COURSE [YSDA Natural Language Processing course (Yandex)](https://github.com/yandexdataschool/nlp_course)

## Talks
- #TALK [Introduction to Natural Language Processing - Cambridge Data Science Bootcamp](https://www.youtube.com/watch?v=8S3qHHUKqYk)
- #TALK [Rob Romijnders | Using deep learning in natural language processing (PyData)](https://www.youtube.com/watch?v=HVdPWoZ_swY)
- #TALK [Jeff Abrahamson - WTF am I doing? An introduction to NLP and ANN's](https://www.youtube.com/watch?v=7Z3ojkuul9U)
- #TALK [Natural Language Processing with PySpark](https://www.youtube.com/watch?v=AsW0QzbYVow)
- #TALK [Feeding Word2vec with tens of billions of items, what could possibly go wrong? (Simon Dollé)](https://www.youtube.com/watch?v=qYpdW9cyEqY)
- #TALK [Deep Learning for Natural Language Processing (2015)](https://www.youtube.com/watch?v=tdLmf8t4oqM)


## Code
- #CODE [Arabica](https://github.com/PetrKorab/Arabica) - A Python package for exploratory analysis of text data
- #CODE [Rubrix](https://github.com/recognai/rubrix) - Rubrix, open-source framework for data-centric NLP. Data annotation and monitoring for enterprise NLP
- #CODE [Beir](https://github.com/UKPLab/beir) - Heterogeneous Benchmark for Information Retrieval
	- #PAPER [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of Information Retrieval Models (Thakur 2021)](https://arxiv.org/abs/2104.08663)
- #CODE [FastText](https://fasttext.cc/) - Library for efficient text classification and representation learning
	 - [Install FastText on Google colaboratory](https://colab.research.google.com/notebook#fileId=1MikDdEIDzFVpH7V6ZSTho8bwOALEmUoa)
- #CODE [Fairseq](https://github.com/facebookresearch/fairseq) - Facebook AI Research Sequence-to-Sequence Toolkit written in Python
	- Fairseq(-py) is a sequence modeling toolkit that allows researchers and developers to train custom models for translation, summarization, language modeling and other text generation tasks
- #CODE [OpenNMT-tf](https://github.com/OpenNMT/OpenNMT-tf) - OpenNMT-tf is a general purpose sequence learning toolkit using TensorFlow 2
- #CODE [OpenNLP](https://opennlp.apache.org/) - The Apache OpenNLP library is a machine learning based toolkit for the processing of natural language text
- #CODE [Textgen RNN](https://github.com/minimaxir/textgenrnn)
- #CODE [Standford CoreNLP](https://stanfordnlp.github.io/CoreNLP/)
- #CODE [NLTK](http://www.nltk.org/) - NLTK is a leading platform for building Python programs to work with human language data
- #CODE [Textblob](https://textblob.readthedocs.io/en/dev/) - TextBlobis a Python library for processing textual data
	- http://ahmedbesbes.com/how-to-mine-newsfeed-data-and-extract-interactive-insights-in-python.html
	- http://nicschrading.com/project/Intro-to-NLP-in-Python/
	- https://github.com/NSchrading/intro-python-nlp/blob/master/Intro_Python_NLP.ipynb
- #CODE [Spacy](https://spacy.io/) - Industrial-strength NLP
	- #TALK [Matthew Honnibal - Designing spaCy: Industrial-strength NLP](https://www.youtube.com/watch?v=gJJQs47aUQ0)
	- #TALK [Patrick Harrison | Modern NLP in Python (SpaCy and gensim for recommendation-reviews analysis)](https://www.youtube.com/watch?v=6zm9NC9uRkk)
	- https://spacy.io/docs/usage/tutorials
	- https://nicschrading.com/project/Intro-to-NLP-with-spaCy/
	- http://blog.thedataincubator.com/2016/04/nltk-vs-spacy-natural-language-processing-in-python/
- #CODE [ParlAI](http://www.parl.ai/) - A unified platform for sharing, training and evaluating dialogue models across many tasks
- #CODE [Gensim](https://radimrehurek.com/gensim/) - Gensim is a Python library for topic modelling, document indexing and similarity retrieval with large corpora
- #CODE [Spark-NLP](https://github.com/johnsnowlabs/spark-nlp) - State-of-the-art Natural Language Processing library built on top of Apache Spark

### LLMs 
- #CODE [Langchain](https://github.com/hwchase17/langchain) - Building applications with LLMs through composability
	- https://python.langchain.com/en/latest/index.html
	- [LangChain explained - The hottest new Python framework](https://www.youtube.com/watch?v=RoR4XJw8wIc)
	- [LangChain Crash Course - Build apps with language models](https://www.youtube.com/watch?v=LbT1yp6quS8)

### Speech
- #CODE [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) - toolkit for tasks in speech and audio, with the state-of-art and influential models
	- #PAPER [PaddleSpeech: An Easy-to-Use All-in-One Speech Toolkit (Zhang 2022)](https://arxiv.org/pdf/2205.12007v1)            
- #CODE [Whisper](https://github.com/openai/whisper) - Robust Speech Recognition via Large-Scale Weak Supervision
	- https://openai.com/research/whisper

### Web scrapping and cleaning
- #CODE [Requests (For fetching HTML/XML from web pages)](http://docs.python-requests.org/en/master/user/quickstart/)
- #CODE [BeautifulSoup (web scraping data parsing)](https://www.crummy.com/software/BeautifulSoup/)
	- #TALK [Introduction To Web Scraping (with Python and Beautiful Soup)](https://www.youtube.com/watch?v=XQgXKtPSzUI)
- #CODE [LXML (web scraping data parsing)](http://lxml.de/)
- #CODE [Dryscape (web scraping with javascript)](https://dryscrape.readthedocs.io/en/latest/)
- #CODE [Selenium (web scraping with javascript)](http://selenium-python.readthedocs.io/)
- #CODE [Scrapy (web scraping framework)](https://github.com/scrapy/scrapy)
	- https://doc.scrapy.org/en/latest/intro/overview.html
	- Scrapy is an application framework for crawling web sites and extracting structured data which can be used for a wide range of useful applications, like data mining, information processing or historical archival.
	- https://medium.com/@kaismh/extracting-data-from-websites-using-scrapy-e1e1e357651a#.j9hrs2scn
- #CODE [python-ftfy: fixes text for you](http://ftfy.readthedocs.org/)
- #CODE [Arrow - working with dates and times](http://arrow.readthedocs.io/en/latest/)
- #CODE [Beautifier - clean and prettify URLs and email addresses](https://github.com/sachinvettithanam/beautifier)

