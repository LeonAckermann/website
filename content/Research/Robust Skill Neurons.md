---
title: Robust Skill Neurons
draft: false
tags:
  - "#mechinterp"
---
This is a write up of my first ever published research project which was also my Bachelor Thesis.

# some history in natural language processing
Back in 2023, I was interested in the Adversarial Robustness of Large Language Models or LLMs. ChatGPT just came out one year earlier in 2022 so the public was slowly noticing the fast progress in Deep Learning. In research, language modeling had been a concept for decades, just a little more than 70 years. 

> [!info]- What is a language model?
 > A language model predicts the next word given a sequence of words. An [ngram](https://en.wikipedia.org/wiki/N-gram) is the simplest version of a language model which makes use the frequency of words in a text corpus to predict the next word of a sequence of words.

Then the research field field of computational linguistics moved from frequency based methods such as [tf-idf](https://en.wikipedia.org/wiki/Tf%E2%80%93idf) to embedding approaches such as [fastText](https://en.wikipedia.org/wiki/FastText)or the [word2vec](https://en.wikipedia.org/wiki/Word2vec) models. One could go a lot more into detail. Essentially the embedding approaches translate a discrete set of words into a continuous numerical representation. To predict the next word using embedding models, one could simply concatenate all the word embeddings together and compute the [softmax](https://en.wikipedia.org/wiki/Softmax_function) over the entire vocabulary. Embedding models allowed the practitioner to utilize the power of Neural Networks. Later, Recurrent Neural Networks (RNN) the were widely adopted to perform tasks such as Next Word Prediction, Sequence Labeling of Text Classification. The recurrent architecture that solved one of the problems RNN suffered from, the vanishing and exploding gradient problem, was the [LSTM](https://en.wikipedia.org/wiki/Long_short-term_memory). This almost brings us to today, as current Large Language Models such as ChatGPT are built with a specific type of neural network, the [Transformer](https://en.wikipedia.org/wiki/Transformer_(deep_learning)). The parallel nature of the Transformer paired with the enormous power of GPUs and the availability of massive amounts of data made the current progress in Deep Learning possible.

# adversarial robustness and interpretability



