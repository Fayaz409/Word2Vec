# **Text Preprocessing and Word Embedding**

**Purpose**

This code demonstrates the following:

* Text preprocessing techniques for natural language processing tasks.
* Word embedding generation using Word2Vec and FastText models.
* Visualization of word embeddings for understanding semantic relationships.

**Steps**

1. **Data Preparation**
   * Read text data from `.txt` files.
   * Combine the data into a single corpus.
2. **Preprocessing**
    * **Sentence Tokenization:** Split the corpus into individual sentences.
    * **Word Tokenization:** Split sentences into individual words.
    * **Stop Word Removal:**  Remove common words (e.g., "the", "and", "is") that carry less semantic importance.
    * **Lowercasing**: Convert all text to lowercase for consistency.
3. **Word Embedding Models**
    * **Word2Vec:**
        * Train a Word2Vec model to learn word embeddings.
        * Explore word similarities and find the odd word out. 
        * Calculate word-to-word similarity scores.
    * **FastText:**
        * Train a FastText model for word embeddings. 
        * Explore word similarities and find words most similar to a given word.
4. **Visualization**
    * **PCA:** Use Principal Component Analysis (PCA) for dimensionality reduction.
    * **Plotly:** Create 2D and 3D scatter plots to visualize word relationships in the embedding space.

**Dependencies**

* `nltk`
* `gensim`
* `re` (Regular expressions)
* `sklearn`
* `plotly`

**Installation**

```bash
pip install nltk gensim re sklearn plotly
nltk.download('punkt') 
```

**How to Run**

1.  Place your `.txt` files in the project directory. 
2.  Update the file paths in the code if needed.
3.  Run the code. Visualizations will be generated. 

**Example Output**

 * 2D and 3D scatter plots showing the distribution of words in the embedding space. Words with similar meanings will tend to cluster together.

**Customization**

* Experiment with different stop word lists.
* Modify the Word2Vec and FastText model parameters (e.g., `window`, `min_count`, `vector_size`).
* Try different visualization techniques.
