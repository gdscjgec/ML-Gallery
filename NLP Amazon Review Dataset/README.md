## Sentiment Analysis NLP Project
In this Project, Sentiment Analysis is done on Amazon Product Dataset from `tensorflow_datasets` so that `tf.data` and other `tensorflow` operations can be done efficiently.

- In this Project, I have used `amazon_us_reviews/Mobile_Electronics_v1_00` Tensorflow dataset 

[Link to the dataset](https://www.tensorflow.org/datasets/catalog/amazon_us_reviews#amazon_us_reviewsmobile_electronics_v1_00).

- For the Traning purposes,`TFDistilBertForSequenceClassification` is used as it is version of `DistilBERT`. It is a very efficient, fast and smaller version of `BERT`. 
- It is pretrained model so we just freeze some layers and add input and output layers according to our requirements. 
- For Tokenizer, `DistilBertTokenizerFast` is used. 

They are imported from `transformers` module. [Link](https://huggingface.co/transformers/)

### REQUIREMENTS
1. GPU (CUDA installed)
2. Tensorflow (Tensorflow_datasets)
3. `transformers` module
4. `NLTK` (Natural Language Tookit)

### USAGE
1. Import the dataset from the `tensorflow_datasets`.
2. Do some data `cleaning` and `preprocessing`.
3. Make two list namely, `reviews` and `labels`.
4. Split into Train and Test set.
5. Apply Tokenizer and then prepare the encodings.
6. Based on those Encodings, make `train` and `test` set using `tf.data.Dataset` function.
7. Import pretrained `TFDistilBertForSequenceClassification` from transformers.
```python
model = TFDistilBertForSequenceClassification.from_pretrained('distilbert-base-uncased', num_labels = 2)
```
8. Fit the data onto the model, using `Adam` optimizer and the `computed_loss` of the pretrained model.

9. Test it using a test sentence.
10. Output the prediction using `softmax` activation `Negative/Positive` sentiment.

### RESULTS
We got `94.2%` validation accuracy on fitting the dataset onto the prepared model.