# Automated Scoring of Mental Time Travel in German Narratives

A pipeline to automate scoring of mental time travel in German narratives, employing natural language processing. 

## Features
- Translation of German text data into English using three different machine translation approaches
- Scoring of internal and external content according to the Autobiographical Interview (Levine, 2002) using a fine-tuned model by Genugten & Schacter (2024) ([GitHub link](https://github.com/rubenvangenugten/autobiographical_interview_scoring))
- Scoring of internal detail categories using a lexical approach
- Dummy data for code testing

## Usage / Workflow
To run the code (see subfolder **/code**) in the correct order, follow these steps:
1. **Setup environment:** Start with `setup.ipynb` to configure the environment and install necessary dependencies.  
2. **Translate texts:** Run `translation.ipynb` to translate German texts into English using the selected machine translation approaches.  
3. **Automatic scoring:** Execute the notebooks for automatic scoring (`auto-scoring-gs24.ipynb` and `auto-scoring-spacy_ger.ipynb`) to obtain internal and external detail scores.  
4. **Manual scoring comparison (optional):**  
   - Use `label-studio.ipynb` to prepare manual annotations.  
   - Run `processing-manual-scoring.ipynb` to process manual scoring data.

## Proof of Concept
Whether this pipeline yields the intended results was evaluated in a proof-of-concept study. An aggregated dataset and the analysis code are available on OSF: [OSF Project](https://osf.io/z97vj/)
