# What Characteristics Make ChatGPT Effective for Software Issue Resolution? An Empirical Study of Task, Project, and Conversational Signals in GitHub Issues
This repository contains the replication package for the study on analyzing the effectiveness of conversational LLMs, such as ChatGPT, in resolving GitHub issues. It includes the datasets, code, and documentation required to replicate our results and insights.
## Project structure
```md
├── analysis
│   └──  main.ipynb -> notebook file to analyze RQs in our datasets with markdowns that separate each part
├── data_collection
│   └──  main.ipynb -> notebook file to collect issue threads containing chatgpt links
├── datasets
│   └──  conversation_progression -> dataset of rounds of each prompt and answer in each conversation to analyze discourse features
│   └──  LIWC_conversation_progression -> conversation progression dataset with LIWC measures to analyze discourse features
│   └──  conversation_repo_parameters -> repository parameters extracted for each project in the conversation
│   └──  final_annotated_conversations -> final annotated dataset, the result of our manual process for RQ1
│   └──  issue_difficulty_metrics -> final annotated dataset with the results of issue metrics (issue difficulty)
│   └──  issue_types -> final annotated dataset with the results of issue metrics (issue types)
│   └──  initial_dataset -> Initial unfiltered annotated dataset
├── example_conversation
│   └──  Example Conversation.pdf -> an example figure to show the full story behind an issue thread using chatgpt
├── pickle_files
│   └──  pickle files generated for the results of discourse analysis
├── conversation_analysis
│   ├── metrics
│   │   └── linguistic.py -> to analyze linguistic metrics in conversation
│   │   └── structural.py -> to analyze structural metrics in conversation
│   ├── utils
│   │   ├── api_call.py -> patterns of API call
│   │   ├── code_snippet.py -> patterns of code snippets
│   │   └── contractions.py -> a list of contractions
│   │   └── urlmatch.py -> a regex for finding URLs
│   └── .gitignore
```

## How to Use
### 1. Data Collection
Use the data_collection/main.ipynb notebook to collect GitHub issue threads with ChatGPT links.
Ensure you have the necessary API keys for GitHub.

### 2. Dataset Overview
conversation_progression: Use this dataset to analyze conversation evolution across rounds.\
LIWC_conversation_progression: Use this for advanced LIWC analysis.\
conversation_repo_parameters: Understand project-level characteristics of repositories.\
final_annotated_conversations: Access manually annotated conversations for RQ1.

### 3. Analysis
Open analysis/main.ipynb to explore the research questions.
The notebook includes steps for reproducing figures and statistical results.

## 4. Scripts for Analysis
linguistic.py and structural.py for Structural and Linguistic metrics evaluations.
api_call.py, code_snippet.py, contractions.py, and urlmatch.py for preprocessing and feature extraction.

### 5. Example
Refer to example_conversation/Example Conversation.pdf for an illustrative example of issue resolution and its developer-ChatGPT conversation.

### Prerequisites
Python 3.9 or above
Required libraries: Gensim, Pandas, NumPy, Scikit-learn, Matplotlib, NLTK, spaCy, spellchecker
