## Week 1 Report – NLP Foundations

### Goals
- Learn basic text preprocessing: tokenization, stemming/lemmatization ideas, stopword removal, n-grams.
- Try classic text representations: Bag-of-Words and TF-IDF.
- Build a small sentiment classifier to see the full pipeline end-to-end.

### What I did
- Practiced tokenization and padding with Keras `Tokenizer` and compared output sequences.
- Tested stemming using NLTK PorterStemmer and noted how it sometimes over-stems words.
- Removed stopwords with both NLTK and spaCy to see differences in vocab size.
- Built Bag-of-Words with `CountVectorizer` including bigrams to capture short phrases.
- Applied TF-IDF (`TfidfVectorizer`) on sample texts and inspected top-scoring terms.
- Ran a full IMDB sentiment pipeline: cleaned text, TF-IDF features, `LogisticRegression` classifier, evaluation with accuracy/F1, and confusion matrix.

### Key observations
- Tokenization choices change vocabulary size; adding OOV tokens helps stabilize models.
- Stemming can distort words; lemmatization would be safer when meaning matters.
- Stopword removal reduced feature space and slightly improved TF-IDF results.
- Bigrams caught phrases like "not good" which improved sentiment signals versus unigrams.
- TF-IDF + Logistic Regression trained fast and performed reliably on a balanced IMDB subset.

### Files and tools
- Main notebook: `Week 1/week1.ipynb` (preprocessing demos and sentiment classifier).
- Dependencies: `Week 1/requirements.txt` with TensorFlow, datasets, NLTK, spaCy, scikit-learn, numpy.