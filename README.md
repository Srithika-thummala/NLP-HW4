# NLP-HW4

Srithika Thummala
700778790


## Question1

1. **Tokenize:** `wordpunct_tokenize` lowercases the sentence and splits it into words and punctuation.
2. **Remove stopwords:** common words like *are*, *in*, and *and* are filtered out using NLTK's English stopword list.
3. **Stem:** `PorterStemmer` cuts each word down to its root (e.g. *techniques* becomes *techniqu*, *assistants* becomes *assist*).

## Question2

`Attention(Q, K, V) = softmax(Q · Kᵀ / √d_k) · V`

1. Multiply Q by Kᵀ to get similarity scores.
2. Divide by √d_k to keep the scores from growing too large.
3. Apply a stable softmax so each row of weights sums to 1.
4. Multiply the weights by V to get the final output.
