## Week 2 Report: Embeddings & RNNs

### Goals
- Try word embeddings (Word2Vec, GloVe) and visualize them.
- Learn basic recurrent models (RNN, LSTM, GRU, BiLSTM) on a toy task.
- Compare a classic baseline (TF-IDF + Logistic Regression) with a deep model (LSTM) on sentiment.

### What I worked on
- Trained Word2Vec on Brown corpus; checked similar words and a simple analogy.
- Loaded pre-trained GloVe vectors; ran cosine-similarity searches.
- Plotted embeddings in 2D with t-SNE and compared with PCA side-by-side.
- Built character-level text generation models: Simple RNN, LSTM, GRU, and BiLSTM; compared their training curves.
- Mini-project: IMDB sentiment classification with two pipelines:
	- TF-IDF (unigrams + bigrams) + Logistic Regression.
	- Tokenizer + padded sequences + stacked LSTM with dropout.
- Measured accuracy, F1, timing, confusion matrices; tested on custom review snippets.

### Key observations
- Word2Vec trained quickly on Brown but vocabulary coverage is limited; pre-trained GloVe is richer.
- t-SNE shows local clusters more clearly; PCA is better for global spread but less clustered.
- LSTM/GRU handled the character task better than a plain RNN; BiLSTM adds parameters but learned context both ways.
- On IMDB subset, TF-IDF + LR was fast and strong; LSTM improved contextual handling but cost more time.

### Files and tools
- Notebooks: `word_embeddings.ipynb`, `lstm_rnn_basics.ipynb`, `mini_project_comparison.ipynb`.
- Dependencies listed in `requirements.txt` (tensorflow, datasets, gensim, nltk, scikit-learn, numpy, matplotlib).

