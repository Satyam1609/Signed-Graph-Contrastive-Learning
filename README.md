# Signed-Graph-Contrastive-Learning

- Link to the paper - https://dl.acm.org/doi/pdf/10.1145/3459637.3482478





## Data

- This file contains the implemetation of Signed Graph Contrastive learning on Bitcoin_alpha dataset available on https://snap.stanford.edu/data/soc-sign-bitcoin-alpha.html  

- bitcoin_alpha\soc-sign-bitcoinalpha.csv -  contains the original data converted to csv format conatining information about the nodes and labels.
- bitcoin_alpha\user_dict.pkl - contains dicionary of all the unique nodes present in the data.
- bitcoin_alpha\g_train.pkl - contains the dictionary of following format -:
"items
(('user', 'positive', 'user'), (array([    0,     1,     2, ...,  7800,  1854, 10135]), array([  483,   483,   483, ..., 10192, 10192,  4365])))
items
(('user', 'negative', 'user'), (array([  119,   120,   121, ...,  2727, 10059,  7112]), array([ 483,  483,  483, ..., 9547, 9496, 1854])))"
here positive and negative indicate the sign of edges and users denotes the nodes.
- bitcoin_alpha\label_train.pkl - it contains the csv file on which training has to be done .

## Code

- IPYNB file - sgcl_bitcoin_alpha.ipynb
- this code can run for other datasets as well mentioned in the repo by just changing the folder name in the code .


## Subparts in the code 

- Importing necessary libraries
- Load user and features
- Load Train Graph
- Load Labels 
- Model definition 
- Graph Augmentation 
- Define Predictor
- Training Parameter Setting
- Training 
- Results from SGCL 
### Training on Logistic Regression, SVM and RandomForest on embeddings using various functions.
i. HADAMARD
ii. Concatenated
iii. L1-normalization
iv. L2-normalization 
v. Averages



