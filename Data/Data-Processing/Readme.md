# Overview
1. Data-Query: Organize Your Folder Structure
* Objective: Prepare and arrange your working directory for efficient data handling.
* Action: Ensure that all necessary files and folders are appropriately structured in your project directory.

2. Data-Preprocessing: Generate Output File
* Objective: Preprocess the raw data to prepare it for further analysis.
* Action: Execute the driver_m.py script. This script processes the raw data and generates an intermediate file named "output_file". This file contains essential features extracted from the data and is crucial for the next step of the analysis.

3. Data-Processing: Run Analysis and Generate Report
* Objective: Analyze the preprocessed data to extract insights.
* Action: Run the classifier_m.py script, which utilizes the "output_file" generated in the previous step. The classifier_m script performs the data analysis and generates a comprehensive report titled "report.txt". This report contains the detailed results and findings of the analysis.


## How Preprocessing Works

To initiate the machine learning process, driver_m.py serves as the primary driver function for data processing and feature extraction. Initially, the script retrieves text-based data identified as speaker="CHI" from the XML folder. The data is processed in three distinct forms: normal, replaced, and stemmed. This tripartite method enhances feature detection accuracy, enabling the algorithm to more effectively identify patterns. Ultimately, such a method would prepare us to run the ultimate machine learning process: classifier_m.py.

### Processing Methods:
- **Normal**: Utilizes the original text to accurately measure the children's language skills.
- **Replaced**: Converts unconventional or unique expressions into a commonly understood language, facilitating an analysis of deviation from standard language use.
- **Stemmed**: Generalizes different word forms to a common base form, simplifying analysis by reducing lexical diversity.

### Examples:
| Method    | Description | Original Text Example | Processed Text Example |
|-----------|-------------|-----------------------|------------------------|
| Normal    | Original text without alterations. | "Saw big big dog. Dog, dog, dog... nice dog." | "Saw big big dog. Dog, dog, dog... nice dog." |
| Replaced  | Substitutes non-standard expressions with standard language. | "Saw big big dog. Dog, dog, dog... nice dog." | "Saw a big dog. It was a nice dog." |
| Stemmed   | Reduces words to their root form. | "Running, jumped, swimming." | "Run, jump, swim." |

Further data extraction was performed focusing on several key aspects: the Child's Words with POS Tags, the Child's Sentences/Uncategorized Utterances, and the sentences/utterances spoken by investigators. Additionally, the Child's Sentences were processed in Plain Text format. These extractions leveraged functions from features.py and LanguageModel.py to ensure comprehensive and detailed analysis.

### output_file Set Description:

Each feature extracted from the data is listed in the order they are appended to the `current_features` array. The values represent computed metrics for linguistic analysis.

Example: 56 4 150 1 1 -3.64 1 3 31 1 52 263 0 0 0 0 0.64 1 1 1 1
<sup><sub>one line from the whole data</sub></sup>

| Feature Number | Description | Example Value(s) |
|----------------|-------------|------------------|
| 1              | Total Number of Words | 56 |
| 2              | Number of Different Words | 4 |
| 3              | Total Number of Utterances | 150 |
| 4              | Mean Length of Utterance (MLU) | 1 |
| 5              | Average Number of Syllables per Word | 1 |
| 6              | Flesch-Kincaid Score | -3.64 |
| 7              | Raw Verbs vs. Total Verbs Ratio | 1 |
| 8              | Number of Different POS Tags | 3 |
| 9              | Number of Repeated Words/Phrases | 31 |
| 10             | Number of Partial Words | 1 |
| 11             | Number of Filler Words | 52 |
| 12             | Degree of Conversational Support | 263 |
| 13             | Prosody Measurement | 0 |
| 14             | Average Number of Clauses per Sentence | 0 |
| 15             | Average Left Branching Dependency | 0 |
| 16             | Maximum Parse Tree Height | 0 |
| 17             | Language Model Probability: Unigram | 0.64 |
| 18             | Language Model Probability: Bigram | 1 |
| 19             | Language Model Probability: Trigram | 1 |
| 20             | Language Model Probability: 4-gram | 1 |
| 21             | Category Label (SLI, ASD, TYP) | 0 OR 1 OR 2 |

## How Processing Works
