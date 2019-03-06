<h1 align="center"> Word Embedding </h1>
the collective name for a set of language modeling and feature learning techniques in natural language processing (NLP) where words or phrases from the vocabulary are mapped to vectors of real numbers.
So, the vector, which reflects the structure of the word in terms of word-context(s) representation, global corpus statistics, words hierarchy in terms of WordNet terminology

<h2 align = "center"> Glove (Global Vectors for Word Representation) </h2>
Tge approach of global word representation is used to capture the meaning of one word embedding with the structure of the whole observed corpus; word frequency and co-occurence counts are the main measures om which the majority of unsupervised algorithms are based on.GloVe model trains on global co-occurrence counts of words and makes a sufficient use of statistics by minimizing least-squares error and, as result, producing a word vector space with meaningful substructure. Such an outline sufficiently preserves words similarities with vector distance.</br>
<h2><a href = "https://towardsdatascience.com/word-embeddings-exploration-explanation-and-exploitation-with-code-in-python-5dac99d5d795" > Tutorial Link </a></h2>


<h2 align = "center"> Keras </h2>
<li> Split Words with text_to_word_sequence </li>
<li> Encoding with one_hot </li>
<li> Hash Encoding with hashing_trick </li>
<li> Tokenizer API </li>
<h2> <a href = "https://machinelearningmastery.com/prepare-text-data-deep-learning-keras/"> Tutorial Link </a> </h2>
 *** Personal notebook track (06/03/2019)

<h3> Keras Functions </h3>
<h4> texts_to_sequences()  </h4>
Only top "num_words" (most frequent words) will be taken into account only words known by the tokenizer will be taken into account.
<h4> pad_sequences()</h4>
pad_sequences is used to ensure that all sequences in a list have the same length. By default this is done by padding 0 in the beginning of each sequence until each sequence has the same length as the longest sequence.