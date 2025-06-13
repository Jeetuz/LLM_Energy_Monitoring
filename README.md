# LLM-Based Code Generation for Energy Data Analysis

This project demonstrates automated Python code generation and execution for energy data analysis using Large Language Models (LLMs) via the Groq API.

## Dataset

- **Source:** [UCI Individual Household Electric Power Consumption](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)

- **File:** `household_power_consumption.txt` (must be present in the working directory)

## Features

- Uses LLMs to generate and execute Python (pandas) code for real-world energy analytics
- Supports natural language queries for:
  - Monthly/daily aggregations
  - Peak usage analysis
  - Weekday/weekend comparisons
  - Correlation and trend analysis
  - Data visualization with matplotlib

## Setup

1. Pull the repository in your VS Code

2. Install requirements:
    ```
    pip install -r requirements.txt
    ```

3. Obtain a [Groq API key](https://console.groq.com) and set it in your notebook or environment.

## Usage

- Run the Jupyter notebook or Python script.
- The system will:
  - Load and preprocess the dataset
  - Prompt the LLM for code generation using your queries
  - Execute the generated code and display results
  - Evaluate each query for correctness or errors

## LLM Used

- **Model Used:** `llama-3.1-8b-instant`,`gemma2-9b-it`,`llama-3.3-70b-versatile`,`llama3-70b-8192`,`llama3-8b-8192`

## Author
- Jeet Parab

## Notes

- See the notebook for detailed query prompts and outputs.
- Notebook Dryrun_Solution_Script.ipynb contains Basic Implementation during intial LLM tryout by me.
- Notebook Optimised_Solution_Script.ipynb contains a similar script with tweaked prompts with evaluation criteria being code or error generated along with type of error which caused the error.
- Notebook LLM_Generated_Solution_Script.ipynb contains script generated via LLM to improvise the prompt quality along with iterating over multiple models available over Groq API to generate response of each model to a query then generate a similar report to the earlier notebook.

---
