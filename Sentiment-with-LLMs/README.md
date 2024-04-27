# Sentiment-with-LLMs
Sentiment Classification through a pre-train and fine-tune BERT paradigm

## About
As Language Models do not have enough context information for downstream tasks like sentiment classification, Masked Language Modeling by masking tokens that are more sentiment-related can prove useful. These Sentiment Tokens can be computed using various methods like topic modeling, TF-IDF, or even manually. In this code, we use the Log-Odds Ratio to compute these tokens and then Mask 15% of input tokens accordingly. The model is then fine-tuned on the training dataset. This code uses the twitter samples dataset provided by NLTK and achieves an F1 score of around 0.7. <br>
This model is inspired by the [Knowledge Enhanced Masked Language Model](https://aclanthology.org/2021.naacl-main.376/) paper 
