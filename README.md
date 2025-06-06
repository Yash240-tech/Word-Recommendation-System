# Word-Recommendation-System

"Word Recommendation System for English Language" project is to create an intelligent system that simplifies and enhances the writing process. This system addresses the challenge of finding suitable and contextually accurate words by providing real-time suggestions based on prefixes and contextual probabilities. By combining efficient data structures and language models, it ensures precise and relevant word recommendations.

The project’s primary objective is to deliver a fast, user-friendly solution that improves writing speed and accuracy. The system leverages the Trie data structure for quick word retrieval and integrates Bigram and Trigram models for contextual accuracy. By analyzing initially typed characters and their sequence, the system predicts and suggests the most relevant words with their probabilities to the user. 
Algorithms discussed

1.	Trie Data Structure for Word Storage: Store words efficiently and support quick word lookup, prefix search, and bigram/trigram-based word prediction.
•	STEPS:
	Initialize Trie: Create a Trie root node and initialize structures for storing unique words and bigrams/trigrams.
	Insert Words: Insert words into the Trie using a CSV file containing unique words.
	Corpus Processing: Read the corpus file and process the text to generate bigrams and trigrams for word predictions.
	Word Lookup: Use the Trie to store and search for words and prefixes that match user input.
 
2.	Bigram/Trigram Processing Algorithm: Process the corpus to generate bigrams and trigrams for improved word prediction accuracy.
•	STEPS:
	Read the Corpus: Read through a corpus of text (e.g., sentences) to extract word sequences.
	Generate Bigrams: For each pair of consecutive words, store them as a bigram (two words together) and track their frequencies.
	Generate Trigrams: Similarly, generate trigrams (sequences of three consecutive words) and track their frequencies.
	Store bigram/trigrams: Store the bigrams and trigrams in appropriate data structures (like HashMaps) for efficient retrieval during predictions.
 
3.	Word Prediction Algorithm: Predict the next word based on user input, leveraging bigram and trigram models.
•	STEPS:
	Input Processing: Accept a user’s input, consisting of a prefix, the last word typed, and optionally, the second-to-last word.
	Match Prefix: Search the Trie to find words that match the input prefix and Select Prediction Model based on-
o	If only one word is provided (last word), use the bigram model to predict the next word based on the preceding word.
o	If both the last and second-to-last words are provided, use the trigram model to predict the next word based on the two preceding words.

4.	Calculate Probabilities: Use frequency data from bigrams and trigrams to calculate the probability of each word being the next in the sequence, applying smoothing techniques for rare or unseen words.

5.	Return Suggestions: Display the predicted words with their probabilities for the user to choose from.
  
6.	User Interface Algorithm: Provide a simple interface for users to input their text and receive word predictions.
•	STEPS:
	Accept User Input: Prompt users to input a word prefix, the last word, and optionally the second-to-last word for more accurate predictions.
	Display Suggestions: After processing the input, display the predicted words, including the probability of each prediction.



