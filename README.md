# Multiple-Instance-Learning-Data-Challenge-Owkin

The challenge proposed by Owkin is a weakly-supervised binary classification problem. Weak supervision is crucial in digital pathology due to the extremely large dimensions of whole-slide images (WSIs), which cannot be processed as is. The chalenge from Owkin lasts for 5 days. 

## Business case:

The goal is to assist with an automatic detection of breast cancer in small image patches taken from larger digital pathology scans.
Usually, with supervised learning algorithms, the learner receives labels for a set of instances. Since a slide is given a single binary annotation (presence or absence of mutation) and is mapped to a bag of tiles, one must learn a function that maps multiple items to a single global label. This framework is known as multiple-instance learning (MIL).

## Data Input
For each patient, we provided three types of input:

the set of (maximum 1,000) tile images randomly chosen inside the tissue as .jpg files
the feature vectors extracted from each of the tiles using a pre-trained resnet model
metadata related to the original slide image.

## Metric
Outputs must be float numbers between 0.0 and 1.0 which represent the probability of PIK3CA mutation. 
The metric for the challenge is the Area Under the ROC Curve (AUC)

# Main Challenges
The two main challenges were:
- Weakly supervised learning
- Handling data from different sources
- About 340 patients. This is a small number compared to the number of patients we want to analyze with our algorithm after its deployment. 

#### Getting started
The notebook below, provided by google collab.


| Description       | Google Colab                                                              |
|-------------------|---------------------------------------------------------------------------|
| Notebook  | https://colab.research.google.com/drive/1_wNEjoX8-_1iSWh9XDlPn_rEHKX14t0H#scrollTo=uXDeOac1CNsU|
