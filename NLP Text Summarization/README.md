# NLP Text Summarization
In this project, we have used `extractive summarization`. It works by identifying important sentences and reproducing them as the summary.
In this approach, no new text is generated, only existing text is used in this process.

- We will use `nltk` library for `Corpus` and `Tokenizers`.
    
    1. `Corpus`:- A collection of words is Corpus.
    2. `Tokenizer`:- It divides the text into a series of tokens. We will be using the word and sentence tokens.

- We are `stopwords`. They are the words which do not add value to a sentence.

## Working
1. A frequency table can be created for the words occuring after removing the stopwords using `dict`.
2. By using this `dict`, we can check which sentence is the most relevant in the whole dataset.
3. Assign `score` to the sentence according to its occurance.
4. One simple approach that can be used to compare the scores is to find an average score of a particular sentence. 
5. This average score can be a good `threshold`.
6. Apply the `threshold` value and the store sentences in an order into the `summary`.

## USAGE
I used an Narrative essay from this [link](https://examples.yourdictionary.com/essay-examples.html)

Run the script for the `summary`
```python
python TextSummarization.py
```

NOTE: If you want to add your own text just simply replace it with the `text` variable.