# Sentiment-analysis
This Project analyzes the scripts of the famous series Rick & Morty.
The aim of the project is to provide a sentimental analysis and predict the mood of each character at each sentence.
-we used SentimentIntensityAnalyzer which is a class in Natural
Language Toolkit (NLTK) library for Python that is used to analyze
and determine the sentiment of text data.

**About Data**.
-our dataset is basically a set of columns each one include a
specific information in the famous series Rick and Morty as the
episode name and a line from that episode with the name of the
character that said it.
-our aim is to figure the mood of the character based on the lines of
the series by using sentimental analysis.

**Preprocessing**.
1\we started cleaning our data and dropping the null and duplicated values.
2\we ranked the unique values of the name column.

3\we created a wordcloud for all the data columns-A word cloud is a visualization technique used to represent text data,
where the size of each word indicates its frequency or importance in the dataset.

4\we then started Preprocesses the movie script text.
-Lowercasing: Converting all text to lowercase helps in standardizing the text data, ensuring that the same word is treated consistently regardless of its capitalization. 
-Removing Stopwords: Stopwords are common words like "and", "the", "is", etc., which occur frequently in the language but typically do not carry much sentiment or meaning. 
 Removing stopwords can reduce noise in the data. 
-Removing Punctuation: Punctuation marks such as periods, commas, and quotation marks often do not contribute significantly to sentiment analysis and can be removed to simplify the text.

**SentimentIntensityAnalyzer**.
-It employs a lexicon-based approach to sentiment analysis, where each word in the text is assigned a sentiment score, typically ranging from -1 (very negative) to 1 (very positive), with 0 representing neutral sentiment. 
-This sentiment analyzer is commonly used in tasks such as social media monitoring, customer feedback analysis, and opinion mining to gauge the sentiment expressed in textual data. It provides a quick and easy way to assess the overall sentiment polarity of a piece of text. 
-we used TF-IDF vectorization (Term Frequency-Inverse Document Frequency) vectorization is a technique used to convert textual data into numerical vectors, which can be understood by machine learning algorithms. It's commonly used in natural language processing (NLP) tasks, including text classification.

**TF-IDF vectorization**.
-TF-IDF vectorization is widely used in text mining tasks such as text classification, information retrieval, document clustering, and keyword extraction. It allows machine learning algorithms to work with textual data by representing documents in a numerical format.
-TF-IDF vectorization converts each document in the corpus into a numerical vector, where each component of the vector represents the TF-IDF weight of a term in the document.
-The resulting vectors are typically high-dimensional and sparse, as they contain mostly zeros due to the presence of many terms in the vocabulary and the rarity of terms in individual documents.

**Multinomial Naive Bayes**.
-Multinomial Naive Bayes (MNB) is a variant of the Naive Bayes algorithm specifically designed for text classification tasks, where the features are typically word counts or term frequencies. It's widely used in natural language processing (NLP) applications, including sentiment analysis, spam detection, and document classification. 
-we will notice that the accuracy given by that algorithm is 69%

**Tkinter**.
-Tkinter is the standard GUI (Graphical User Interface) toolkit for Python. It provides a set of tools and libraries to build graphical applications with a rich set of user interface components such as buttons, labels, text entry fields, and more. 
-Tkinter is based on the Tk GUI toolkit, which originated as part of the Tcl scripting language, but has been ported to many programming languages including Python. Tkinter is known for its simplicity and ease of use also it  can run on various operating systems such as Windows, macOS, and Linux without modification.

**ttk from Tkinter**.
-stands for "themed Tkinter" and is an extension module that provides themed widgets for Tkinter, Python's standard GUI toolkit such as buttons, labels, entry fields, comboboxes, notebooks, progress bars, and more. It is part of the standard library starting from Python 3.1. The ttk module aims to enhance the appearance and functionality of Tkinter widgets, providing a more modern and consistent user interface.

**messagebox from Tkinter**.
-The messagebox module in Tkinter provides a simple way to display various types of message boxes or dialog boxes in GUI applications. These message boxes are commonly used to present information, ask for confirmation, or prompt the user for input.
-we will provide our model with a certain piece of the dialogue from the movie said by one of the characters and it will give us the mood of that character.

**Filedialog from Tkinter**.
-The filedialog module in Tkinter provides a set of dialogs for file operations, allowing users to interactively select files or directories in GUI applications. These dialogs are commonly used for tasks such as opening files, saving files, and selecting directories. 

**Conclusions**.
-By analyzing the performance of the model we will notice that it classify the mood of
the characters whether it is positive ,negative or neutral based on the piece of the
dialogue provided.
-In summary, sentiment analysis involves analyzing text to determine sentiment,
which can be approached using machine learning algorithms like Naive Bayes, with
text represented using techniques like TF-IDF vectorization. Tkinter provides a
convenient way to build GUI applications, including those for sentiment analysis,
allowing users to interact with the analysis results in an intuitive and user-friendly
manner.
