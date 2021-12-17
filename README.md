# Research Paper Tagger (RPT)

This repository is tested on Python 3.7.12 and TensorFlow 2.7.0

### Dataset:

The dataset can be found [here](https://github.com/arbaazQureshi/research_paper_tagger/tree/main/Data).

The dataset split which was used in our project is can be accessed from the [Splits](https://github.com/arbaazQureshi/research_paper_tagger/tree/main/Data/Splits) folder


### TF-IDF Baseline model:
To run this model:
1.	Install the required scikit-learn package by running the below command on terminal:
	```python	
	pip install scikit-learn
	```
2.	Run the [tf-idf.ipynb](https://github.com/arbaazQureshi/research_paper_tagger/blob/main/Models/tfidf/tf-idf.ipynb) obtain the predictions and evaluation results.


### RNN Baseline model:
To run this model:

1.	Install the required packages by running the below command on terminal:
	```python
	pip install tensorflow
	```
	```python
	pip install keras
	```
	```python
	pip install pandas
	```
	```python
	pip install numpy 
	```
	```python
	pip install nltk 
	```
	```python
	pip install scikit-learn
	```
2.	Download the word2vec tool from the [Google's code archive](https://code.google.com/archive/p/word2vec/): 
	
	 [GoogleNews-vectors-negative300.bin.gz](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?usp=sharing)
3.	Run the [RNN_word2vec.ipynb](https://github.com/arbaazQureshi/research_paper_tagger/blob/main/Models/RNNs/RNN_word2vec.ipynb) notebook in the RNN folder to obtain the predictions and evaluation results.

### RPT Model

To run the RPT model:

1.
