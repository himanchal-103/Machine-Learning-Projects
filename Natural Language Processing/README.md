# NATURAL LANGUAGE PROCESSING

## Objective
1. The primary objective of this project is to develop a comprehensive system for extracting and analyzing textual data from articles available at specified URLs. The project encompasses two main tasks: data extraction and text analysis.
2. Data Extraction:
    1. Input Source: The URLs of the articles are provided in an Excel file named Input.xlsx.
    2. Extraction Process: For each article URL listed in Input.xlsx, extract the article's title and text.
    3. Ensure that only the article title and text are extracted, excluding any website headers, footers, or other extraneous content.
    4. Save the extracted article text into a text file named after the URL_ID provided in the Input.xlsx file.
3. Data Analysis: Perform textual analysis on each of the extracted articles to compute the listed variables.
    - Positive Score
    - Negative Score
    - Polarity Score
    - Subjectivity Score
    - Average Sentence Length
    - Percentage of Complex Words
    - Fog Index
    - Average Number of Words per Sentence
    - Complex Word Count
    - Word Count
    - Syllables per Word
    - Personal Pronouns
    - Average Word Length
4. Output Requirements: The results of the analysis should be saved in the format specified by the Output Data Structure.xlsx file.

## Metrics to be calculated with their formulas:
The document outlines the methodology for performing text analysis, focusing on sentiment, readability, and various linguistic metrics. Here's a summary of the key points:

1. Sentimental Analysis:
  - Cleaning: Use stop word lists to exclude common, non-informative words.
  - Dictionary Creation: Use a master dictionary to compile lists of positive and negative words, excluding stop words.
  - Derived Variables: Calculate four key metrics:
    - Positive Score: Sum of +1 for each positive word.
    - Negative Score: Sum of -1 for each negative word (multiplied by -1 for positive scoring).
    - Polarity Score: (Positive Score – Negative Score) / (Positive Score + Negative Score + 0.000001).
    - Subjectivity Score: (Positive + Negative Scores) / (Total Words after cleaning + 0.000001).

2. Readability Analysis
- Gunning Fog Index: Measures text complexity.
  - Average Sentence Length: Total words / total sentences.
  - Percentage of Complex Words: Complex words / total words.
  - Fog Index: 0.4 * (Average Sentence Length + Percentage of Complex Words).

3. Additional Metrics
- Average Number of Words Per Sentence: Total words / total sentences.
- Complex Word Count: Words with more than two syllables.
- Word Count: Total words after removing stop words and punctuation.
- Syllable Count Per Word: Vowels per word, with exceptions for endings like "es" and "ed".
- Personal Pronouns: Count "I", "we", "my", "ours", and "us" using regex, excluding "US" (the country).
- Average Word Length: Total characters in words / total words.

These methods combine to analyze the sentiment and readability of texts, providing insights into their complexity, tone, and linguistic features.
