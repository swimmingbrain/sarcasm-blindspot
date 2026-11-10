# Sarcasm Blindspot

Lab project for the AI and Visualization course at JKU, by team **AI-West**.

## Idea

**How does removing hashtags and emojis affect a model's ability to detect irony?**

Tweets often contain hashtags like `#sarcasm`, `#irony`, or `#not` that provide clues about their intended meaning.

We want to investigate how much Twitter-RoBERTa relies on these cues to detect irony and whether removing them affects ironic and non-ironic tweets differently.

## Model and Data

- **Model:** [Twitter RoBERTa Irony](https://huggingface.co/cardiffnlp/twitter-roberta-base-irony) by Cardiff NLP, used without further training.
- **Dataset:** [TweetEval – Irony](https://huggingface.co/datasets/cardiffnlp/tweet_eval), using the test set containing 784 tweets (311 ironic and 473 non-ironic).
- **Hypothesis:** Removing hashtags and emojis changes the model's predictions and confidence differently for ironic and non-ironic tweets.

We compare four modifications:
1. Remove hashtags.
2. Remove emojis.
3. Remove both hashtags and emojis.
4. Remove only the `#` symbol while keeping the hashtag word.

## Phases

**Phase I: How does the model behave?**

We treat the model as a black box and compare its original predictions with predictions after modifying the tweets.

We investigate changes in predicted irony labels, prediction probabilities, and differences between ironic and non-ironic tweets. We use three visualizations and selected tweet examples to examine the model's behavior in more detail.

**Phase II: What did the model learn?**

We plan to investigate the model's internal behavior using techniques such as Integrated Gradients and UMAP projections.

Our goal is to understand whether the model relies heavily on explicit irony cues like hashtags or also considers the broader context of a tweet.

In each phase, one pair works with generative AI tools and the other pair works without them. We compare both approaches at the end of each phase.

## Team

- Cedric Hempe
- Erik Ludescher
- Braian Plaku
- Lukas Steu
