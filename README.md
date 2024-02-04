**Prerequisites**

Before running the notebook, ensure you have the following:

- Python 3.6 or newer installed on your system.
- Jupyter Notebook or JupyterLab installed. You can install it via pip with pip install notebook or pip install jupyterlab.

**Part 1 Instructions:**
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Dataset** : CUAD\_v1.zip

This dataset consists of 510 text files, each containing a full-text contract. These files are in plaintext format and are named following the pattern [document name].txt. The contracts are not labeled.

**Input Files:**

1. 'merged.txt' Contains all 510 files merged together
2. 'stopwords.txt' Contains the stopwords provided for the assignment

**Code :** NLP\_Assignment\_Part1.ipynb contains the code

**Dataset Output Folder :**

1. 'output.txt' contains all the tokens
2. 'tokens.txt' contains a list of all tokens and their frequencies

For viewing the output, any browser can be used.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Part 2 Instructions:**

**Dataset** : sts2016-english-with-gs-v1.0

This package contains test sets with gold standard labels for the 2016 Semantic Textual Similarity (STS) shared task.

**Input Files**

    STS2016.input.answer-answer.txt

    STS2016.input.headlines.txt

    STS2016.input.plagiarism.txt

    STS2016.input.postediting.txt

    STS2016.input.question-question.txt

**Gold Standard Files:**

    STS2016.gs.answer-answer.txt

    STS2016.gs.headlines.txt

    STS2016.gs.plagiarism.txt

    STS2016.gs.postediting.txt

    STS2016.gs.question-question.txt


**Code :** The Code folder contains all sentence embedding models we used.

    Doc2vec.ipnyb 

    InferSent.ipnyb

    roberta.ipnyb

    sbert_mpnet.ipnyb

    universal_sentense_encoder.ipnyb

Open google collab upload the dataset files and the .ipnyb notebook. Change the readline file and execute to see the output list of cosine similarities.

** To run InferSent.ipnyb models.py should also be uploaded to collab


**Dataset Output Folder :**

    The cosine similarity list files and the gold standard files are stored under this folder.

    To execute the perl script and get the persson coeff run the below command:

    /correlation-noconfidence.pl STS2016.gs.<dataset>.txt  <model>.txt
