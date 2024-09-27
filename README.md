# README: Probing Transformer-Based Neural Network Models for Alzheimer's Disease Screening

## Overview
This project investigates the potential of transformer-based language models, such as DistilBERT, for early Alzheimer's disease (AD) screening through speech analysis. The study explores connections between biolinguistic theory and machine learning models, probing whether these models can detect linguistic markers of AD as identified by biolinguistic research. 

This project was carried out in the context of the **Language Engineering course for the Master's in Artificial Intelligence (MAI)**.

## Key Objectives
1. **Bridge Biolinguistic Theory and Language Models**:  
   - Use large language models (LLMs) to screen for AD while grounding predictions in biolinguistic theory.
   - Investigate whether LLMs, which often function as black-box models, can provide insights aligned with biolinguistic research on language decline in AD patients.
   
2. **Adversarial Probing Task**:  
   - Fine-tune DistilBERT for AD prediction based on speech transcripts from the ADDReSS 2020 dataset.
   - Create adversarial examples for different biolinguistic variables to test if the LLM can detect linguistic markers known to correlate with AD (e.g., delayed language production, word frequency, syntactic simplifications).

## Dataset
- **ADDReSS 2020 Dataset**:  
   A subset of the Pitt DementiaBank corpus, consisting of speech transcripts from AD patients and control groups.

## Methodology
- **Fine-tuning Models**:  
   DistilBERT was fine-tuned using logistic regression classifiers. Leave-one-out (LOO) cross-validation was employed due to the small dataset size.
   
- **Probing Experiments**:  
   A minimalist probing task was conducted by creating adversarial test samples to determine if the language model recognizes specific semantic, syntactic, and pragmatic features related to AD.

## Key Findings
- **Sensitivity to Semantic Features**:  
   The probing task showed that DistilBERT is particularly sensitive to semantic markers of AD, such as the use of high-frequency words, indefinite terms, and delayed language production.
   
- **Limited Response to Syntactic Features**:  
   Syntactic and pragmatic markers, such as referential cohesion and inflectional errors, showed limited significance, suggesting these features may be harder for the model to detect or operationalize.
   
- **Implications for Biolinguistic Theory**:  
   The results support some biolinguistic hypotheses, such as Lust et al.'s (2018) claim that AD affects the syntax-semantics interface before core syntactic capacities.

## Conclusion
This project represents an initial step toward integrating biolinguistic theory with machine learning models in AD detection. The results suggest that combining linguistic theory with LLMs holds promise for enhancing explainability in clinical applications. However, further research with larger datasets and more refined experiments is needed.

## Citation
If you use this work, please cite:
- **Anonymous Submission
