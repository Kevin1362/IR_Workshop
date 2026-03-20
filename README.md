# IR Inverted Matrix Workshop Solution

This project contains a solved version of the **IR Inverted Matrix Workshop**. It implements tokenization, normalization, a positional inverted index, phrase query search, IDF, TF, and a simple TF-IDF comparison.

## Team Members

- Kevinkumar Patel -8998612
- Prajesh Bhatt - 9026277

## Project Files
- `ir_inverted_matrix_workshop_solution.py` — cleaned Python script with comments
- `IR_InvertedMatrix_Workshop_Solved.ipynb` — solved Jupyter notebook version
- `requirements.txt` — packages needed to run the project
- `IR_InvertedMatrix_Workshop_Notes.md` — summary notes and talking points
- `ir_inverted_matrix_workshop_solution_output.txt` — sample output

## Dataset Description
This solved version is designed to run **without internet access**.

Instead of depending on a live RSS feed, the script creates an **offline fallback corpus** inside the Python file:
- 20 text documents
- more than 2000 unique words
- repeated phrase patterns such as `information retrieval`, `machine learning`, and `inverted index`
- additional synthetic terms to make the vocabulary large enough for the workshop requirement

This makes the project reliable and easy to run on any laptop, even if the internet is blocked or the original RSS feed is unavailable.

## Dataset Link and License
### Default dataset used in this project
- **Dataset source:** Generated locally inside `ir_inverted_matrix_workshop_solution.py`
- **Public link:** Not required
- **License:** Not applicable because the fallback corpus is generated in the code for educational use

### Optional original workshop source
The original workshop notebook suggested collecting text from a public RSS source:
- **Example RSS source:** `https://pyfound.blogspot.com/feeds/posts/default?alt=rss`
- **Use in this solved version:** Optional only; not required to run the project
- **License:** Check the original publisher terms before redistributing scraped content

## Features Implemented
- Document collection / fallback corpus
- Tokenizer
- Stop-word removal
- Stemming
- Positional inverted index
- Phrase query search
- Optimized positional index idea
- IDF calculation
- TF calculation
- TF-IDF table output

## How to Run

### 1. Create a virtual environment (recommended)
#### Windows
```bash
py -m venv .venv
.venv\Scripts\activate
```

#### macOS / Linux
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2. Install requirements
```bash
pip install -r requirements.txt
```

### 3. Run the Python solution
```bash
python ir_inverted_matrix_workshop_solution.py
```
If your computer uses `py` instead of `python`, run:
```bash
py ir_inverted_matrix_workshop_solution.py
```

## How to Run the Notebook
```bash
jupyter notebook
```
Then open:
```text
IR_InvertedMatrix_Workshop_Solved.ipynb
```

## Expected Output
When you run the script, it will print:
- number of loaded documents
- vocabulary size
- sample tokens
- normalized tokens
- preview of the positional index
- phrase query results
- sample positional postings
- IDF value for a sample term
- TF and TF-IDF table
- TF vs IDF comparison table
- final talking point about bigram search

## Notes
- The script tries to use **NLTK stopwords** and downloads them automatically if needed.
- If `pandas` is installed, the TF and TF-IDF results are printed in a cleaner table.
- If you add your own `.txt` files into a folder named `sample_docs`, the script can read those instead of the generated fallback corpus.

## Submission Tip
If you upload this project to GitHub, include:
- your final team member names
- your course / section if required
- your GitHub repository link in the email to the instructor
