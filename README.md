# Peptide-Classification
Developed and trained a predictive neural networks that can determine, given an antibacterial peptide, whether it is also an antibiofilm peptide.
## Description
Biofilms are tightly-connected multicellular communities of microorganisms encased in self secreted extra-cellular matrices. They are currently one of the major causes of disease for two main reasons. First, roughly 75% of all human infections are caused by biofilms. Second, due to the robust multicellular cellular matrix structure, they are resistant both to
the host defense mechanisms and to traditional antimicrobial compounds (antibiotics).
Thus, it is important to identify peptide sequences that are not only antimicrobial, but also antibiofilm.
<br> This repository contains all the code and datasets.
## Data Description
train.dat is used for training and test data test.dat consisting of peptide sequences, one per line in the file. Peptides are encoded as strings with characters
from an alphabet of 20 characters, each representing an amino-acid residue. The training set also includes the label for each sequence as 1 (antibiofilm) or -1 (not antibiofilm) as the
first character in each line of the training file, separated from the sequence by a tab (\t) character.
## Approach
* Used K-mers for feature extraction 
* Used imbalanced-learn python library for oversamplin the imbalanced dataset
## Results
* Train Accuracy: 1.0
* Validation Accuracy: 0.97
* MCC Score on test data: 0.8642
