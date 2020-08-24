# Janatahack-Independence-Day-2020-ML-Hackathon
 
This repository contains **9th place** solution to [Janatahack-Independence-Day-2020-ML-Hackathon](https://datahack.analyticsvidhya.com/contest/janatahack-independence-day-2020-ml-hackathon/) organised by Analytics Vidhya

## Problem Statement

### Topic Modeling for Research Articles

Researchers have access to large online archives of scientific articles. As a consequence, finding relevant articles has become more difficult. Tagging or topic modelling provides a way to give token of identification to research articles which facilitates recommendation and search process.

Given the abstract and title for a set of research articles, predict the topics for each article included in the test set.

Note that a research article can possibly have more than 1 topic (Multilabel Text Classification). The research article abstracts and titles are sourced from the following 6 topics:

1. Computer Science

2. Physics

3. Mathematics

4. Statistics

5. Quantitative Biology

6. Quantitative Finance

## Evaluation Metric 

  Micro F1 score
  
## LeaderBoard 

- [Public LB](https://datahack.analyticsvidhya.com/contest/janatahack-independence-day-2020-ml-hackathon/#LeaderBoard): **0.8528076199** & **8th out of 364 submissions**
- [Private LB](https://datahack.analyticsvidhya.com/contest/janatahack-independence-day-2020-ml-hackathon/#LeaderBoard): **0.849371161158233** & **9th out of 364 submissions**

  
## Approach

-  Trained 3 models using ULMFiT, BERT and RoBERTa 

- Final Submission was generated using `Ensembles`  notebook.

- Created a Voting Classifier of the following for final submission as it performed better on Public LB.:
1. *BERT* 
2. *Weighted avg of predictions of ULMx0.4 and BERTx0.6* 
3. *Avg of predictions of 3 models* 
4. *Weighted avg of predictions of 3 models (ULMx0.35 BERTx0.45 RoBERTax0.20)*  


| **Model**  | **Public LB  Score**| **Private LB Score** |  
|---|---|---|
| ULMFiT |0.83904|0.84314	|
| BERT |0.84517|0.83979	| 
| RoBERTa |0.83581|0.83779| 
|Avg of predictions of 2 models| 0.84982 | 0.84819 |
|Avg of predictions of 3 models| 0.85121 | 0.84984 |
|Weighted avg of predictions of 3 models| 0.85185 | 0.85067 |
|Voting Classifier of best 4|0.85281|0.84937|




