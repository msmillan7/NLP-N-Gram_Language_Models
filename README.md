# NLP-N-Gram_Language_Models

In this project we use the DUC 2005 dataset to assess the performance of three n-gram language models (where n = 2, 3, and 4) with and without Laplace-k smoothing. 

The code is written within jupyter notebooks, which allowed us to have one pipeline (or notebook) to perform each specific task. Thus, the outputs fo the first pipeline are saved and used as inputs to the next pipeline and so forth. This allows for easy compiling and running of the code:   
1. Clone the folder from GitHub. 
2. Navigate to the folder from within your terminal. 
3. Open up an editor including Jupyter Lab or Visual Studio Code that allows for execution of jupyter notebooks. 
4. Run the cells of the notebooks sequentially.

## Contents

The project contains four pipelines (jupyter notebooks) that each of them performing a specific task:
- NLP-Assignment_1-preprocessing_training.ipynb: includes the preprocessing of the training data and generates the following outputs, that will be used in the next pipelines:
  - unknown_words.txt: List of words tagged as \<UNK\> during the preprocessing.
  - used_words.txt: List of unique words after preprocessing.
  - training_sentences.pkl: List of sentences in the training set after preprocessing, before tagging \<UNK\> words.
  - training_sentences_unk.pkl: List of sentences in the training set after preprocessing, after tagging \<UNK\> words.
  - unigram_dictionary_training.pkl: Dictionary containing all the unigrams of the training set after preprocessing.
  - bigram_dictionary_training.pkl: Dictionary containing all the biigrams of the training set after preprocessing.
  - trigram_dictionary_training.pkl: Dictionary containing all the triigrams of the training set after preprocessing.
  - fourgram_dictionary_training.pkl: Dictionary containing all the fourgrams of the training set after preprocessing. 

- NLP-Assignment_1-preprocessing_testing.ipynb: includes the preprocessing of the test data and generates the following outputs, that will be used in the next pipelines:
  - test_sentences.pkl: List of sentences in the test set after preprocessing, before tagging \<UNK\> words.
  - test_sentences_unk.pkl: List of sentences in the test set after preprocessing, after tagging \<UNK\> words.
  - unigram_dictionary_test.pkl: Dictionary containing all the unigrams of the test set after preprocessing.
  - bigram_dictionary_test.pkl: Dictionary containing all the biigrams of the test set after preprocessing.
  - trigram_dictionary_test.pkl: Dictionary containing all the triigrams of the test set after preprocessing.
  - fourgram_dictionary_test.pkl: Dictionary containing all the fourgrams of the test set after preprocessing.

- NLP-Assignment_2-analysis.ipynb: Includes summary statistics of the training and test datasets and a use case of the application of smoothing on some bigrams.

- NLP-Assignment_3-results.ipynb: includes the functions to calculate the likehoods, probabilities and perplexities of the different N-Gram Models. It also contains a specific analysis for three random sentences picked from the training set.
