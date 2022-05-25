# PDF TEXT Summarizer for Metals and Minerals Standard

A Comprehensive extraction of PDF file methods, and various Deep Learning Algorithms for text Summarizer.

The model should be able to extract the sections like Introduction, Sustainability disclosures topics… and sub sections like Greenhouse Gas emission, Air Quality etc and it’s relevant text and summarize it.

## Data Set

PDF file is downloaded from the link: https://www.sasb.org/wp-content/uploads/2018/11/Metals_Mining_Standard_2021.pdf

## Pre-requisites

1. Register in the open-ai and get api key, and org key from https://beta.openai.com/account/api-keys.
   set the below propeties in the notebook.

   ```javascript
   OPEN_AI_ORG = "org-example-id";
   OPEN_AI_API_KEY = "OPEN-API-KEY";
   ```

2. Create directory structure under `results` for running evaluation and debugging.

   ```bash
       # bash command
       mkdir "results/model_evaluation/debug"
   ```

## Steps to Run

1. Downlod the pdf file and keep it under resource directory.

2. Run all cells in `Metals_Mining_Standard_2021_Summary.ipynb` notebook.

3. The output of summary is generated and saved in path `results/summary/Metals_Mining_Standard_2021_Summary.txt`.

## Fun Next Steps

- Explore more on BLEU and ROGUE metrics to apply and evaluate the models.

- Evaluate model for tabular data.

## Resources

[1] Open AI: https://beta.openai.com/docs/guides/completion/introduction

[2] Bert sentence transformers Models: https://huggingface.co/sentence-transformers?sort_models=likes#models

[3] Bert Extractive Summarizer: https://pypi.org/project/bert-extractive-summarizer/

[4] Evaluation Metrics for Text Summarization: https://www.researchgate.net/publication/220106310_Evaluation_Measures_for_Text_Summarization#:~:text=The%20summarization%20systems%20are%20ranked,summary%20with%20its%20full%20text.

[5] Huggingface Summarization: https://huggingface.co/tasks/summarization
