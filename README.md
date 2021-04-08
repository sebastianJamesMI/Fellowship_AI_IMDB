Fellowship_AI_IMDB

Colab Notebooks for IMDB Task

This project uses the IMDB dataset compiled by Andrew Maas (see http://ai.stanford.edu/~amaas/data/sentiment/).

The objective is to classify movie reviews as positive or negative. The original reviews were rated on a scale from 1 to 10. For Binary Classification, anything with <= 4 was classfed as negative and anything with >= 7 stars were classified as positive.
I use different strategies to perform this classification task starting with a simple RNN model (LSTM) then using more complex models. This notebook uses a simple Baseline model and references the following sources:

1. Google official Tensorflow page on text classification using BERT: https://www.tensorflow.org/tutorials/text/classify_text_with_bert
2. Data Reading and Downloading: Georgios Drakos: https://gdcoder.com/sentiment-clas/
3. Word Tokenization: Coursera Deep learning NLP courses by Andrew Ng
4. Using CNN for NLP tasks: NLP course on Udemy by Martin Jocqueviel: https://www.udemy.com/course/modern-nlp/
5. Data reading and downloading, Aaron Kub: https://towardsdatascience.com/sentiment-analysis-with-python-part-1-5ce197074184

I used models of increasing complexity to do the classification task


1. Baseline: Using Tensorflow Tokenizer with a simple Neural Network (NN): Sentiment_Analysis_IMDB_Baseline.ipynb
2. Using the Tensorflow Tokenizer with LSTM layers: Sentiment_Analysis_IMDB_TF_Tokenizer_LSTM.ipynb
3. Using the BERT Tokenizer with a CNN layers: Sentiment_Analysis_IMDB_BERT_Tokenizer_CNN.ipynb
4. Using the BERT Tokenizer and fine-tuning a BERT layer: Sentiment_Analysis_IMDB_BERT_Embedding_LSTM.ipynb
5. Using the Official Tensorflow tutorials on using BERT:Sentiment_Analysis_IMDB_Tensorflow_Tutorial.ipynb
6. Fine tuning Keras BERT API: Sentiment_Analysis_IMDB_BERT_Hub_Layer.ipynb


Model Number	Model*****************************************Accuracy (1 = 100%)
1.	Simple Neural Network (NN)*******************************0.81
2.	Tensorflow Tokenizer with LSTM layers*********************0.85
3. 	BERT Tokenizer with a CNN layers**************************0.89
4. 	BERT Tokenizer and fine-tuning a BERT layer***************0.88
5. 	Using Tensorflow Official BERT Tutorial*********************0.85
6. 	Fine tuning Keras BERT API*********************************0.93
