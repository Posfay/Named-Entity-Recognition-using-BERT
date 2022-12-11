# Named Entity Recognition using BERT

Homework for VITMAV45 by Team PBP: Alex Papp (JG18IB), Benedek Pósfay (CDJEOZ)

We are using hunNERwiki, a Hungarian corpus for Named Entity Recognition (NER). The goal of the project is to create and train a model for NER using transfer learning and a pretrained version of BERT as a starting point.

## Data Preprocessing
First, we download the corpus and organize it into one dataset and perform some data manipulation. Since the size of the dataset is relatively large, we save the modified version for further use (due to GitHub having a file size limit and the data preprocessing taking too much time, we did not upload the final dataset to the repository. However you can download the resulting dataset - later used for training - from [here](https://drive.google.com/drive/folders/16kM3YkZtdVLYffU40EdvKCEKrXCpIDtj?usp=share_link)). The notebook for the data preprocessing can be found [here](https://github.com/Posfay/Named-Entity-Recognition-using-BERT/blob/main/NER_Data_Preprocessing_and_Tokenization.ipynb).

## Training and Evaluation
For the training procedure, we need to tokenize our dataset (encode the input text into a format that BERT accepts). We have used two different models for tokenizing our data: huBERT, a Hungarian BERT cased model and RoBERTa, a multilingual and lightweight version of BERT. Then we trained both models for NER on the tokenized data. The fine-tuned model is then evaluated with official NER metrics and comparisons between models can easily be made. The notebook responsible for training huBERT can be found [here](https://github.com/Posfay/Named-Entity-Recognition-using-BERT/blob/main/NER_Training_and_Evaluation.ipynb) and the notebook for training RoBERTa is available [here](https://github.com/Posfay/Named-Entity-Recognition-using-BERT/blob/main/RoBERTa_NER_Training_and_Evaluation.ipynb).
