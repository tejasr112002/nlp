# Part 1: Named Entity Recognition

![nlp_1](https://github.com/tejasr112002/nlp/assets/73415129/bad2ba7c-1121-4967-a0c2-372608365032)
The above image shows a sample sentence as input into our model. The output is as expected since we use the BIOES tagging scheme and the named entities here are "Wang" tagged as S-PER and "Nanyang Technologoical Univesity" tagged as B-ORG, I-ORG, and E-ORG.

Question_1_NER.ipynb - This notebook contains all the source codes for Part 1 of the assignment. It has the following sections: 

1. Data Preprocessing
2. Model Building
3. Hyperparameter Tuning
4. Final Model Building
5. Testing our model on a random test sentence

Note : The notebook was run on google colab therefore we saved the word2vec model on google drive after the first download so that we do not need to redownload it multiple times. To run on your local PC please uncomment the line where the word2vec model is downloaded using the gensim downloader and please comment out the lines where we are loading the model in from our google drive

# Part 2: Question Classification

![nlp_2](https://github.com/tejasr112002/nlp/assets/73415129/b23fdf85-73af-4bc4-a61e-912f67e0a172)
The above image shows a sample test sentence. Our model classifies it as 'HUM' for Human as expected.

Data_Preprocessing.ipynb - This notebook contains the code for data preprocessing of Part 2 of the assignment. 
In this notebook, we are reading the TREC Dataset,selecting 4 classes of 6, splitting the dataset into training and development, and getting word2Vec embeddings of input text features and storing them to google drive for future use. 

Model_Training.ipynb - This notebook contains the code for experimentation of all the aggregation methods and the final model is trained and tested on unseen data.

Hyperparameter_bLSTM.ipynb - This notebook contains code for the hyperparameter tuning to find the best parameters for the Bi-Directional LSTM model.

Hyperparameter_Transformer.ipynb - This notebook contains code for the hyperparameter tuning to find the best parameters for the Transformer model.
