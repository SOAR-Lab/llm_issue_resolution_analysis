# LLM Conversation Analysis
## Project structure
```md
├── analysis
│   └──  main.ipynb -> notebook file to analyze RQs in our datasets with markdowns that separate each part
├── datasets
│   └──  conversation_progression -> dataset of rounds of each prompt and answer in each conversation to analyze discourse features
│   └──  LIWC_conversation_progression -> conversation progression dataset with LIWC measures to analyze discourse features
│   └──  conversation_repo_parameters -> repository parameters extracted for each project in the conversation
│   └──  final_annotated_conversations -> final annotated dataset, the result of our manual process for RQ1
│   └──  initial_dataset -> Initial unfiltered annotated dataset
│   └──  LIWC_conversation_progression -> Initial unfiltered annotated dataset
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
