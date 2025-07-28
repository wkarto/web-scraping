# Web Scraping and NLP with Requests, BeautifulSoup, and spaCy

This project showcases a complete workflow for web scraping and text mining using Python. It demonstrates how to scrape an article from the web, extract clean text content, and perform natural language processing (NLP) with `spaCy`.

## Features
- Scrape and save article HTML using `requests` and `BeautifulSoup`
- Extract plain text using `.get_text()`
- Analyze token and lemma frequencies using `spaCy`
- Score sentences based on token and lemma occurrences
- Visualize sentence scores using histograms
- Filter and analyze only specific parts of speech (e.g., nouns)

## How to Use This Repository

1. Clone this repository.
2. Install required dependencies using:

   ```bash
   pip install -r requirements.txt
   ```

3. Open `notebook.ipynb` using Jupyter Notebook or JupyterLab.
4. Run the notebook cell by cell and follow the comments.

## Repository Contents

- `notebook.ipynb`: Main Jupyter Notebook with all questions and code.
- `article.html` or `article.pkl`: Saved HTML content of the article (Question 1).
- `README.md`: This documentation file.
- `requirements.txt`: List of Python dependencies used in the notebook.

---

## Summary of Questions & Output

### ✔ Question 1
- Article HTML is saved to a separate file and pushed to the repository.

### ✔ Question 2
- Clean text extracted using `.get_text()` and printed successfully.

### ✔ Question 3
**Top 5 Most Frequent Tokens:**
1. comment — 136  
2. march — 133  
3. 2021 — 133  
4. says — 132  
5. report — 130  

### ✔ Question 4
**Top 5 Most Frequent Lemmas:**
1. comment — 157  
2. say — 134  
3. march — 133  
4. 2021 — 133  
5. report — 130  

### ✔ Question 5
- Sentence scoring function implemented for both token and lemma approaches.
- Correct score for the first sentence printed from both methods.

### ✔ Question 6
- Histogram plotted for token-based sentence scores with appropriate title and axis labels.

### ✔ Question 7
- Histogram plotted for lemma-based sentence scores.
- Highest sentence frequency observed around score range 4 to 6.

### ✔ Question 8
- **Omitted Words When Filtering Nouns:**  
  Words like "says" or "said" (verbs), "quickly" (adverb), and other non-noun types would be excluded.

- **Code Change:**  
  Modify the loop with:
  ```python
  if token.pos_ == "NOUN":
      # process token
  ```

---


