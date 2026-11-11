# Khmer Word Segmentation

A beginner-friendly Python notebook that segments Khmer text using a dictionary and a Trie. It scans a sentence from left to right and selects the longest dictionary word it can find. This is a dictionary-based method, not a machine-learning model.

## What it shows

- The original Khmer sentence
- The segmented sentence
- Each recognized word and its part of speech
- The sentence with zero-width spaces between words
- The total number of word tokens
- Repeated words and how many times they occur
- Khmer text that was not found in the dictionary

## Requirements

- Python 3
- Visual Studio Code
- The Jupyter extension for VS Code
- A Khmer dictionary CSV file

The notebook uses Python's standard library, so no additional Python packages are required.

## Set up the dictionary

Place your dictionary at:

```text
data/khmer_dictionary.csv
```

The CSV should have a `word` column. A `pos` column is optional. If your file uses different column names or a different location, update `WORD_COLUMN`, `POS_COLUMN`, and `DICTIONARY_CSV` in the notebook's settings cell.

Dictionary data is excluded from this Git repository. Only add or share dictionary data if you have permission to do so.

## Run the notebook

1. Open `Khmer_Word_Segmentation.ipynb` in VS Code.
2. Select a Python kernel if prompted.
3. Run the cells from top to bottom.
4. In the sentence input cell, replace the sample text with your Khmer sentence.
5. Run the final cell to see the segmentation results.

## Limitations

The segmenter depends on the words in its dictionary. Unknown Khmer text is kept in the output and listed as unmatched. Longest-match dictionary segmentation may not always choose the linguistically correct word boundaries.
