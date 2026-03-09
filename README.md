[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/code-joswin/dna-promoter-classifier/blob/main/Promoter_Classifier.ipynb)
# DNA Promoter Sequence Classifier

A machine learning project that classifies DNA sequences as 
promoter regions or non-promoter regions using the E. coli 
promoter dataset from UCI Machine Learning Repository.

## What is a Promoter?
A promoter is a region of DNA that signals RNA Polymerase 
to start transcribing a gene. Finding promoters is a 
fundamental problem in bioinformatics.

## What I Built
- Logistic Regression baseline
- 1D CNN with Global Max Pooling
- 1D CNN with Local Max Pooling

## Results
| Model | Accuracy |
|-------|----------|
| Logistic Regression | 91% |
| CNN Global Max Pool | 92% |
| CNN Local Max Pool  | 87% |

## Key Finding
The CNN independently rediscovered the TATAAT motif — 
the known E. coli promoter consensus sequence — without 
being given any biological knowledge. Two filters (34 and 38) 
learned this pattern purely from labeled sequence data.

## Dataset
UCI ML Repository — E. coli Promoter Gene Sequences
106 sequences, 57 nucleotides each, balanced classes.

## Tools
Python, PyTorch, scikit-learn, pandas, matplotlib
