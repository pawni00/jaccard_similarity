# jaccard_similarity
A Python project to calculate the Jaccard Similarity between datasets
# Word Similarity & Spelling Corrector using Jaccard Similarity

A lightweight Python implementation of a spelling correction engine. This project utilizes **Character N-grams** and the **Jaccard Similarity Coefficient** to find and suggest the closest matching correct words from a dictionary for misspelled inputs.

## 🚀 Features

- **Text Preprocessing:** Cleans and normalizes text input (lowercasing, special character removal).
- **Character N-grams:** Breaks words down into overlapping substrings (bi-grams by default) to capture structural similarity.
- **Jaccard Similarity Evaluation:** Computes the mathematical closeness between word structures.
- **Auto-Correction:** Automatically maps misspelled words (e.g., `machin`, `scince`) to their closest correct dictionary forms.

---

## 🧠 How it Works

### 1. Jaccard Similarity Formula
The Jaccard index measures the similarity between two finite sample sets (in this case, sets of character n-grams) and is calculated as:

$$J(A, B) = \frac{|A \cap B|}{|A \cup B|}$$

*   **Intersection ($A \cap B$):** Common n-grams between both words.
*   **Union ($A \cup B$):** Total unique n-grams across both words.

### 2. N-gram Example
For the word `"university"` with $n=2$ (Bi-grams):
```python
['un', 'ni', 'iv', 've', 'er', 'rs', 'si', 'it', 'ty']
