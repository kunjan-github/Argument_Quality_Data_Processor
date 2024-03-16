# Computational Argumentation 2022 -- Assignment 1

This repository contains Python code for processing the "Dagstuhl-15512-ArgQuality" corpus, which involves downloading the corpus, extracting relevant data, storing it as JSON, and creating data splits for machine learning tasks.

## Tasks

1. **Download the Corpus**
    - The "Dagstuhl-15512-ArgQuality" corpus should be downloaded for running the provided code.

2. **Extract Relevant Data and Store as JSON**
    - Extract relevant information per argument from the corpus, including:
        - Argument ID
        - Issue
        - Stance on the issue
        - Argumentativeness annotations (from all three annotators)
        - Quality scores (from all three annotators)
        - Effectiveness scores (from all three annotators)
        - Argument text
    - Store the extracted data in JSON format.

3. **Create Data Splits**
    - Split the extracted data into three subsets for training ML models:
        - Training set
        - Test set
        - Validation set
    - Perform a 70-20-10 percent split for train-test-validation.
    - Ensure no duplicates exist (i.e., the same argument in two splits).

4. **Data Export**
    - Export the combined arguments as a JSON file in the format presented in the previous step.
    - Export the splits into separate files, e.g., `train.json`, `test.json`, and `val.json`.

## Usage

1. Clone this repository:

    ```bash
    git clone <repository-url>
    ```

2. Download the "Dagstuhl-15512-ArgQuality" corpus and place it in the appropriate directory.

3. Run the Python script to process the corpus and create data splits:

    ```bash
    python main.py
    ```

4. After execution, you will find the following files generated:
    - `combined_arguments.json`: JSON file containing all extracted arguments.
    - `train.json`, `test.json`, `val.json`: JSON files containing training, test, and validation data splits, respectively.

## Requirements

- Python 3.x
- XML ElementTree (`xml.etree.ElementTree`)
- JSON (`json`)
- OS (`os`)
- Random (`random`)

## Note

Ensure that the corpus directory structure matches the expected structure in the code. Adjust paths if necessary.
