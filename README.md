# Research Paper Tagger (RPT)

This repository uses Python 3.9.7

### Dataset:

The dataset can be found [here](https://github.com/arbaazQureshi/research_paper_tagger/tree/main/Data).

The dataset split which was used in our project is can be accessed from the [Splits](https://github.com/arbaazQureshi/research_paper_tagger/tree/main/Data/Splits) folder


### RPT models:

1. All the RPT models can be found in 'Models/BERT'. RPT is trained on different combinations of title, abstract, and author names. All of these combinations can be found in the 'Models/BERT' subdirectory. The names of the folders under this subdirectory are intuituve enough (RPT-title lies in the subdirectory 'Models/BERT/Title', RPT-title-abstract-authors lies in the subdirectory 'Models/BERT/AbstractAuthorsTitle')

2. In order to run these models, go to the research_paper_tagger directory, and create a new conda environment through the command line argument:

	```python	
	conda create --name NLP --file package-list.txt
	```

    Next, activate the environment:

	```python	
	conda activate NLP
	```

3. The code for training and validation is present in the jupyter notebook RPT.ipynb. You just have to run the cells of this notebook in order, to train your model.

4. To see how RPT performs on your own paper, go to the directory 'RPT demo'. Then, input the title of the paper in 'Title.txt', the abstract in 'Abstract.txt', and the author names in 'Authors.txt'. Ten run the cells of the RPT.ipynb notebook in order. You will get 3 research track recommendations for your input at the last cell.

5. The code for data extraction is present in 'DatasetBuilding/' subdirectory, in the notebook 'DatasetExtraction.ipynb'. Dataset collection was a semi manual and semi automatic process, so the code for collecting the data, in the 'DatasetBuilding/' is not universal; it might not run for other years' ACL papers. After you successfully run all the cells of DatasetExtraction.ipynb, run DataBaking.ipynb in order to get the data splits and the metadata dictionaries.

6. The error analysis of RPT-title-abstract-authors lies in the subdirectory 'Error analysis/AbstractAuthorsTitle'. Run the cells in order, to examine the misclassified examples, and to generate the T-SNE cluster visualisations.


### TF-IDF baseline model:
To run this model:
1.	Install the required scikit-learn package by running the below command on terminal:
	```python	
	pip install scikit-learn
	```
2.	Run the [tf-idf.ipynb](https://github.com/arbaazQureshi/research_paper_tagger/blob/main/Models/tfidf/tf-idf.ipynb) obtain the predictions and evaluation results.


### RNN baseline model:
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