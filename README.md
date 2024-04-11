# Generative AI for First-Aid Instructions (RAG Model Experiments)

This repository contains the code and data used in our research paper comparing RAG and RAFT for generating first-aid instructions in emergencies. The focus here is on the RAG model experiments.

## Abstract:
The paper explores the potential of Retrieval-Augmented Generation (RAG) for first-aid guidance. RAG allows Large Language Models (LLMs) to access external knowledge bases during response generation. We investigate the effectiveness of RAG in this context and analyze its strengths and limitations compared to RAFT, a fine-tuned approach.

## Getting Started:

1. Clone this repository.
2. Install the required dependencies: pip install -r requirements.txt
3. Download the pre-trained LLM models (OpenAI GPT-3, Google Gemini API) as per their respective instructions.
- (Optional) Replace knowledge_base.pdf with a structured medical knowledge base if available.
4. Run the training script: python rag_model.py --train
5. Run the evaluation script (modify arguments as needed): python rag_model.py --evaluate --test_data test_data.json

## Further Exploration:

- Experiment with different LLM models for RAG.
- Explore alternative knowledge base formats for potentially richer information retrieval.
- Implement additional filtering mechanisms to address potential hallucinations in RAG outputs.

## Usage
Currently, pre-trained models are not provided due to potential safety concerns with using RAG for first-aid guidance. The provided code demonstrates the training and evaluation process. You can train your own RAG model with the provided data following these steps:

Modify rag_model.py to specify your chosen LLM (e.g., OpenAI API, Google Gemini API) and its access credentials.
Run the script python rag_model.py train to train the RAG model.
Run the script python rag_model.py to evaluate the model's performance on the test scenarios.

## Disclaimer:

The provided code and data are for research purposes only. The authors are not responsible for any misuse of this information. Always consult a medical professional in case of a real emergency.
