# T5-Medical at SemEval-2024 Task 2: Using T5 Medical Embedding for Natural Language Inference on Clinical Trial Data
This repo contains data and code for our article: "T5-Medical at SemEval-2024 Task 2: Using T5 Medical Embedding for Natural Language Inference on Clinical Trial Data". 
For a detailed description of our code, please see the article published at SemEval2024, by M.Siino, 2024.

## Abstract
In this work, we address the challenge of identifying the inference relation between a plain language statement and Clinical Trial Reports (CTRs) by using a T5-large model embedding. The task, hosted at SemEval-2024, involves the use of the NLI4CT dataset \cite{jullien2023nli4ct}. Each instance in the dataset has one or two CTRs, along with an annotation from domain experts, a section marker, a statement, and an entailment/contradiction label. The goal is to determine if a statement entails or contradicts the given information within a trial description. Our submission consists of a T5-large model pre-trained on the medical domain. Then the pre-trained model embedding output provides the embedding representation of the text. Eventually, after a fine-tuning phase, the provided embeddings are used to determine the CTRs' and the statements' cosine similarity to perform the classification. On the official test set, our submitted approach is able to reach an F1 score of 0.63, and a faithfulness and consistency score of 0.30 and 0.50 respectively. 

## Code
All the code used in our experiments can be executed on Google Colab.

## BIBTEX
@inproceedings{siino2024t5,  
title = {T5-Medical at SemEval-2024 Task 2: Using T5 Medical Embedding for Natural Language Inference on Clinical Trial Data},
booktitle = "Proceedings of the 18th International Workshop on Semantic Evaluation (SemEval-2024)",
publisher = "Association for Computational Linguistics",
year = {2024},
author = {Marco Siino}  
}
