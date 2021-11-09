# 11711-Reproduce-Results-Topological-Sort-For-Sentence-Ordering

This repository contains results of reproducing results from [Topological Sort for Sentence Ordering](https://arxiv.org/pdf/2005.00432.pdf).  
The authors have published the code accompanying this paper in [GitHub](https://github.com/shrimai/Topological-Sort-for-Sentence-Ordering) 


## Data
We obtained the AAN and NIPS data by mailing the authors of [Sentence Ordering and Coherence Modeling using Recurrent Neural Networks.](https://arxiv.org/pdf/1611.02654.pdf)  
We downloaded the SIND dataset (Stories ofImages-in-Sequence (SIS)) from [Visual Storytelling](http://visionandlanguage.net/VIST/dataset.html) website.  
GloVe embeddings are downloaded from [here](https://nlp.stanford.edu/projects/glove/).  


## Results

### NIPS Abstracts - BTSort
Model | PMR | Acc | Tau | Rouge-S | LCS | Details
------------ | ------------- | ------------ | ------------- | ------------ | ------------- | ------------ 
Reference | 32.59 | 61.48 | 0.81 | 87.97 | 83.45 | 
Reproduced | 32.34 | 62.22 | 0.81 | 87.80 | 82.41 | Used checkpoint-6000

### AAN Abstracts - BTSort
Model | PMR | Acc | Tau | Rouge-S | LCS | Details
------------ | ------------- | ------------ | ------------- | ------------ | ------------- | ------------ 
Reference | 50.76 | 69.22 | 0.83 | 87.76 | 85.92 | 
Reproduced | 50.49 | 68.82 | 0.82 | 87.58 | 85.76 | Used checkpoint-18000

### SIND Captions - BTSort
Model | PMR | Acc | Tau | Rouge-S | LCS | Details
------------ | ------------- | ------------ | ------------- | ------------ | ------------- | ------------ 
Reference | 20.32 | 52.23 | 0.60 | 78.44 | 77.21 | 
Reproduced | 19.12 | 51.45 | 59.1 | 78.08 | 76.51 | Used checkpoint-14000


## Team
1. [Sameer Jain](https://github.com/JainSameer06)
2. [Sunita Selvan](https://github.com/isunitha98selvan)
3. [Vaishakh Keshava](https://github.com/Vaishakh-K)
