# Text Retrieval and Ranking System with TF-IDF and BM25

## Overview

This project implements a text retrieval and ranking system using **TF-IDF** and **BM25** scoring algorithms. The system preprocesses text data, computes document scores based on queries, and retrieves the most relevant documents.

Data Retrieval Course Dr. Mohammadreza Shams
## Features

- **Text Preprocessing**:
  - Lowercase conversion.
  - Removal of stopwords, punctuation, and apostrophes.
  - Stemming using Porter Stemmer.
  - Conversion of numbers to words.
- **TF-IDF Calculation**:
  - Computes TF-IDF scores for both document text and titles.
  - Combines scores with a weighted average for final ranking.
- **BM25 Scoring**:
  - Implements BM25 scoring for document ranking.
  - Uses the `rank_bm25` library for optimized BM25 computation.
- **Query Matching**:
  - Preprocesses user queries and retrieves top-ranked documents based on TF-IDF and BM25 scores.

## Installation

To run this project, ensure you have the following Python libraries installed:

```bash
pip install nltk num2words numpy pandas scikit-learn rank-bm25
```

Also, download the required NLTK data files:

```python
import nltk
nltk.download('stopwords')
nltk.download('punkt')
```

## Usage

1. **Data Loading**:
   - Load text documents and their titles from the specified directory structure.

2. **Preprocessing**:
   - Apply text preprocessing steps to clean and normalize the text data.

3. **TF-IDF Calculation**:
   - Compute TF-IDF scores for document text and titles.

4. **Query Matching**:
   - Use `matching_score` for TF-IDF-based retrieval.
   - Use `matching_score_bm25` or `bm25_matching_score_lib` for BM25-based retrieval.

5. **Document Retrieval**:
   - Retrieve and display the top-ranked documents for a given query.

## Example

```python
matching_score(10, "a lion dont cry")
bm25_matching_score_lib("lions tiger")
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or additional features.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Libraries**: NLTK, Num2Words, NumPy, Pandas, Scikit-learn, Rank-BM25
- **Dataset**: Custom text dataset organized in directories.

## Contact

For any inquiries, please contact **Iman Khalilorahmani** at [imankhtech@gmail.com](mailto:imankhtech@gmail.com).

---
