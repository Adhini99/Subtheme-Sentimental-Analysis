# Subtheme-Sentimental-Analysis
This project performs subtheme sentiment analysis on customer reviews, identifying specific aspects (subthemes) and their associated sentiments. The approach leverages natural language processing (NLP) techniques to extract insights from textual data.

# Features
Preprocessing: Cleans and preprocesses text by removing special characters, numbers, and stopwords, and performs lemmatization.
Aspect Extraction: Identifies key aspects and their descriptors using linguistic patterns.
Sentiment Analysis: Determines the sentiment (positive, negative, neutral) for each aspect using the VADER sentiment analysis tool.

# Technologies Used
Languages: Python

# Libraries:
spaCy: For dependency parsing and named entity recognition (NER).
NLTK (Natural Language Toolkit): For tokenization, stopword removal, and sentiment analysis using the VADER sentiment analyzer.
Pandas: For data manipulation and handling CSV files.
Regex (re): For advanced text preprocessing and cleaning.

# Methods
1.Text Preprocessing:

Tokenization
Stopword removal
Lemmatization
Special character and number removal

2.Aspect Extraction:
Identifies nouns and proper nouns as aspects.
Extracts descriptors using dependency parsing.

3.Sentiment Analysis:
Utilizes VADER to determine sentiment scores.
Classifies sentiments into positive, negative, or neutral based on compound scores.

# Usage
Load and Inspect Data: Load the customer reviews from a CSV file.
Analyze Reviews: Process each review to extract subthemes and sentiments.
Store Results: Add the analyzed subtheme sentiments back into the DataFrame and inspect the results.

# 1.MOTIVATION OF APPROACH
This project provides a streamlined approach to extract and analyze subtheme sentiments from textual reviews, utilizing contemporary NLP techniques and tools. It offers a robust framework for gaining insights from customer feedback, enhancing your understanding of specific aspects and their associated sentiments.

# 2.EXPLANATION OF CODE
# Preprocessing: The preprocess function tokenizes the text, removes stopwords, and converts tokens to lowercase.
# Aspect Extraction: The extract_aspects function uses dependency parsing to identify nouns and objects linked to verbs, indicating potential aspects.
# Sentiment Analysis: The get_sentiment function uses VADER to analyze the sentiment of each identified aspect.
# Review Analysis: The analyze_review function integrates preprocessing, aspect extraction, and sentiment analysis to produce the final subtheme sentiments.

Load and Inspect CSV: The load_data function loads the CSV file without headers (header=None) and prints the first few rows to inspect the structure.
Select Review Column: You need to determine which column contains the reviews. Here, it's assumed that the reviews are in the first column (index 0). Adjust this index based on your CSV structure.
Analyze and Add Results: The script processes each review, analyzes the subthemes and sentiments, and adds the results to the DataFrame.
# Based on the structure of CSV file, it appears that the reviews are located in the first column (index 0) and the subtheme sentiments are listed in the subsequent columns.
Load and Inspect CSV: The load_data function loads the CSV file without headers (header=None). We then print the first few rows to inspect the structure.
Select Review Column: We assume that the reviews are in the first column (index 0) based on your provided structure.
Analyze Reviews: We process each review, analyze the subthemes and sentiments, and store the results in a list.
Add Results to DataFrame: The results are added as a new column ('subtheme_sentiments') to the DataFrame.
# This approach ensures that the analysis is applied to the correct data, and the results are structured in a way that aligns with the original data format. Adjust the column index or name based on your specific CSV file structure if needed.

# 3.IMPROVEMENTS AND POSSIBLE ISSUES
# Contextual Sentiment Analysis: The sentiment analysis could be improved by using more advanced models like BERT, which better understand context.
# Aspect Refinement: The aspect extraction could be fine-tuned to better differentiate between aspects and problems.
# Scalability: The approach should be tested on larger datasets to ensure scalability and efficiency.

# PROBLEMS I FACED
Print Column Names: Before running the analysis, the script prints the column names in the CSV to verify the correct column name for reviews.

Column Existence Check: The script checks if the specified column exists in the DataFrame and raises an error if it does not, guiding you to use the correct column name.

Run Analysis: After verifying the column name, the analysis is run and results are added to the DataFrame.
# we need to correctly handle the CSV file and ensure we are working with the correct column that contains the reviews

# From the provided DataFrame, it appears that the subtheme_sentiments column is being populated with subthemes and their sentiments. However, there might be improvements needed to ensure the analysis is capturing all relevant subthemes and sentiments correctly.

# Improved Code Implementation
Let's enhance the code to improve preprocessing, aspect identification, and sentiment analysis. We will:
Preprocessing: Improved by removing special characters and numbers.
Aspect Identification: Enhanced by including more linguistic patterns for extracting descriptors.
Sentiment Analysis: Refined to handle more nuanced expressions.

# Such updated approach aims to capture a more accurate sentiment analysis by refining each step of the process. Adjust the CSV column index or names based on your specific data structure if needed.



