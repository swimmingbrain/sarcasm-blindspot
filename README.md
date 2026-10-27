# Sarcasm Blindspot

Lab project for the AI and Visualization course at JKU, by team **Green Deranged Titans**.

## Idea

Can a sentiment classifier understand sarcasm?

A tweet like *"Great, another three hour delay!"* is full of positive words but clearly expresses frustration. We want to find out whether a model trained on positive and negative language falls for this, and if so, why.

## Model and data

* Model: [Twitter RoBERTa Sentiment](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment) by Cardiff NLP, used as is without further training
* Data: the sentiment and irony subsets of [TweetEval](https://github.com/cardiffnlp/tweeteval), plus a small set of sarcastic tweets we label by hand with their true sentiment
* Bonus: at the end we might feed the model some of Chandler Bing's sarcastic lines from Friends, taken from [this paper](https://doi.org/10.22146/lexicon.v12i2.109306), to see if it gets them right

## Phases

**Phase I: How does the model behave?**
We treat the model as a black box and compare prediction confidence and sentiment distributions between ordinary and sarcastic tweets.

**Phase II: What did the model learn?**
We open the model up with Integrated Gradients and UMAP projections to check whether it relies on isolated positive words instead of the full context.

In each phase one pair works with generative AI tools and the other pair works without them. We compare both approaches at the end of each phase.

## Team

* Cedric Hempe
* Erik Ludescher
* Braian Plaku
* Lukas Steu
