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
Neural Networks are powerful but of course, they also bring challenges. Two of the biggest problems are:
1. how can we make a neural network generalise to new unseen data and how can we make the model adversarially robust?
> [!info]- what is adversarial robustness?
> Adversarial robustness is measured by changing the input to the network minimally. If the networks output doesn't change compared to no alteration, the network is robust. If the output changes, the network is not adversarially robust.
2. how can we know how a neural network arrives at its answer - this topic concerns the **interpretability** of the network
> [!info]- what is interpretability?
> Neural Networks have been notoriosly called *black boxes*. Interpretability seeks to find out what the learnt network internals represent and how they influence the output of the network

# so what are robust skill neurons?
The title of this post is **robust skill neurons**, so lets talk about them. Skill Neurons are specific neurons within the Feedforward network of the Transformer that show very high or very low activity associated to a specific input and output of the network. Essentially, if those neurons don't function in the network, its performance would degrade drastically. They encode skill. Our research showed that when a network scores well when its tested for adversarial robustness, the same skill neurons are activated as when the input is not altered. In other words, the skill neurons do not only encode skill but also let the model be robust in new unseen scenarios. Tbc

A little bit more

[^ref]

