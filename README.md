# HindiTextGenerator 
# Problem Statement
Our objective is to develop a chatbot with a focus on natural language processing in Hindi, leveraging the indicnlp library. The library provides essential tools for Indian languages, including tokenization and transliteration. Our dataset consists of excerpts from the "Story of Mirabai," written in Hindi.

# Steps Followed:
1. Tokenization:

- Utilized the indicnlp library to tokenize sentences from the "mirabai.txt" file.
- Counted unique word tokens to assess the vocabulary size.
2. Vocabulary Preprocessing:

- Replaced out-of-vocabulary words with "unknown_token" for standardization.
- Demonstrated vocabulary size and showcased examples before and after preprocessing.
3. N-gram Analysis:

- Analyzed the distribution of bigrams, trigrams, quadgrams, etc., to understand linguistic patterns.
- Examined the most common n-grams and their frequencies.
4. Training Data Preparation:

- Prepared training data for a sequence-to-sequence model.
- Implemented the Fisher-Yates shuffle algorithm to randomize data order while maintaining relationships.
5. Extended Training Data:

- Collected and processed additional training data from multiple sets of n-grams.
- Applied the tqdm library to track progress.
6. Sentence Variations:

- Generated sentence variations by extracting the last i words from existing sentences.
- Showcased a random sample of these variations.
7. Word Embeddings:

- Loaded a pre-trained FastText word embedding model using Gensim.
- Created word vectors and a function to find semantically similar words.
8. Sequence-to-Sequence Model:

- Developed a TensorFlow/Keras model using Embedding, SimpleRNN, and Dense layers.
- Trained the model on the prepared training data.
- Analyzed the model's limitations regarding random word insertion, word repetition, and contextual understanding.
9. Alternative Approach:

- Explored an alternative approach from an online article.
- Used Keras Tokenizer for preprocessing and sequence generation.
- One-hot encoded the target words for training.
10. User Interaction:

- Enabled user interaction to input lines of text and predict the next word using the trained model.
- Implemented a loop allowing continuous interaction until the user enters "0."
# Result and Challenges:
Despite achieving high training accuracy, the model demonstrated limitations in random word insertion, word repetition, and contextual understanding. An alternative approach was explored to address these issues, emphasizing the importance of refining model predictions for practical chatbot applications. The steps followed showcase a comprehensive journey in developing and improving the chatbot's language processing capabilities.

# Code Dependencies 
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?logo=tensorflow&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-%23013243.svg?logo=numpy&logoColor=white)
![Pickle](https://img.shields.io/badge/Pickle-%23D00000.svg?logo=python&logoColor=white)
![ModelCheckpoint](https://img.shields.io/badge/ModelCheckpoint-%23150458.svg?logo=python&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?logo=keras&logoColor=white)
![Plot Model](https://img.shields.io/badge/Plot_Model-%23150458.svg?logo=python&logoColor=white)

![Tokenizer](https://img.shields.io/badge/Tokenizer-%23FF6F00.svg?logo=tensorflow&logoColor=white)
![Embedding](https://img.shields.io/badge/Embedding-%23013243.svg?logo=tensorflow&logoColor=white)
![LSTM](https://img.shields.io/badge/LSTM-%23FF6F00.svg?logo=tensorflow&logoColor=white)
![Dense](https://img.shields.io/badge/Dense-%23013243.svg?logo=tensorflow&logoColor=white)
![Sequential](https://img.shields.io/badge/Sequential-%23FF6F00.svg?logo=tensorflow&logoColor=white)
![To Categorical](https://img.shields.io/badge/To_Categorical-%23150458.svg?logo=tensorflow&logoColor=white)
![Adam](https://img.shields.io/badge/Adam-%23013243.svg?logo=tensorflow&logoColor=white)

![Pad Sequences](https://img.shields.io/badge/Pad_Sequences-%23FF6F00.svg?logo=tensorflow&logoColor=white)
![SimpleRNN](https://img.shields.io/badge/SimpleRNN-%23013243.svg?logo=tensorflow&logoColor=white)

![TSNE](https://img.shields.io/badge/TSNE-%23013243.svg?logo=scikit-learn&logoColor=white)
![Spatial](https://img.shields.io/badge/Spatial-%23FF6F00.svg?logo=scipy&logoColor=white)
![Gensim](https://img.shields.io/badge/Gensim-%23013243.svg?logo=gensim&logoColor=white)
![Random](https://img.shields.io/badge/Random-%23189392.svg?logo=python&logoColor=white)
![TQDM](https://img.shields.io/badge/TQDM-%23FF6F00.svg?logo=python&logoColor=white)
![Counter](https://img.shields.io/badge/Counter-%23150458.svg?logo=python&logoColor=white)
![Ngrams](https://img.shields.io/badge/Ngrams-%23FF6F00.svg?logo=nltk&logoColor=white)
![IndicNLP](https://img.shields.io/badge/IndicNLP-%23150458.svg?logo=nltk&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23013243.svg?logo=python&logoColor=white)
