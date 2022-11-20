# Named Entity Recognition using BERT

Homework for VITMAV45 by Team PBP: Alex Papp (JG18IB), Zalán Bokor (T0JVW9), Benedek Pósfay (CDJEOZ)

We are using hunNERwiki, a Hungarian corpus for Named Entity Recognition (NER). The goal of the project is to create and train a model for NER using transfer learning and a pretrained version of BERT as a starting point.

## Data Preprocessing
First, we download the corpus and organize it into one dataset and perform some data manipulation. Since the size of the dataset is relatively large, we save the modified version for further use. The notebook for the data preprocessing can be found [here](https://github.com/Posfay/Named-Entity-Recognition-using-BERT/blob/main/NER_Data_Preprocessing_and_Tokenization.ipynb)

## Training and Evaluation
For the training procedure, we need to tokenize our dataset (encode the input text into a format that BERT accepts). The model we use for tokenizing our data is huBERT, a BERT cased model trained on the Hungarian Webcorpus 2.0 and a snapshot of the Hungarian Wikipedia. This is the same model that we are fine-tuning to achieve better NER results. The fine-tuned model is then evaluated with official NER metrics. The notebook responsible for training can be found [here](https://github.com/Posfay/Named-Entity-Recognition-using-BERT/blob/main/NER_Training_and_Evaluation.ipynb)
