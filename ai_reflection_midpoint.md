# AI Reflection – Phase I

**AI-aided Pair:**
- Cedric Hempe – k12438455
- Erik Ludescher – k52211122

## Our Experience with GenAI

During Phase I, we mainly used ChatGPT to help us with coding, finding a suitable model, creating visualizations, and understanding our results.

At first, we planned to use a sentiment classifier to investigate sarcasm. After looking more closely at the available models and datasets, we realized that an irony detection model would fit our investigation better, so we decided to switch.

AI was especially useful for working with the TweetEval dataset, implementing experiments, and creating visualizations. We investigated how removing hashtags and emojis affects the model's predictions, but also looked at word clusters and how different words influence the detection of irony. ChatGPT helped us implement K-means clustering, create heatmaps, and compare words associated with correct and incorrect predictions.

Based on these findings, we developed additional experiments to investigate the model's sensitivity to linguistic cues. For example, we compared ironic and non-ironic sentences containing the same positive words and tested how removing individual words or punctuation changed the predicted irony probability. AI helped us generate test sentences, implement the comparisons, and interpret the resulting plots.

However, not everything AI suggested worked as expected. Some code contained errors or needed adjustments, and several visualizations were initially too complicated or did not clearly show what we wanted to investigate. We had to refine our prompts, modify the code, and decide which visualizations were actually useful.

We also noticed that AI sometimes suggested interpretations that went beyond what our results could support. For example, identifying word clusters does not necessarily mean that the model internally represents these words similarly. We therefore had to question the explanations, check the results, and design additional experiments to better understand the observed behavior.

Overall, GenAI saved us quite some time, especially with coding, debugging, and developing new ideas for our analysis. It also helped us move from simple visualizations toward more detailed investigations. However, we learned that AI-generated code and interpretations should not be accepted without verification. We still needed to understand the methods, critically evaluate the findings, and make the final decisions ourselves.
