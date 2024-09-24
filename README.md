# text-translation-and-sentiment-analysis-using-transformers
Udacity Deep Learning NanoDegree Project to demonstrate the use of transformers

The objective of this project is to analyze the sentiment of movie reviews in three different languages - English, French, and Spanish. We have been given 30 movies, 10 in each language, along with their reviews and synopses in separate CSV files named movie_reviews_eng.csv, movie_reviews_fr.csv, and movie_reviews_sp.csv.

The first step of this project is to read data from all the .csv files and create a single pandas dataframe. This dataframe should have the following columns - Title, Year, Synopsis, Review, and Original Language.
The next step is to convert the French and Spanish reviews and synopses into English. This will allow us to analyze the sentiment of all reviews in the same language. We will be using pre-trained transformers from HuggingFace to achieve this task.
Finally, we will use pretrained transformers from HuggingFace to analyze the sentiment of each review. The sentiment analysis results (Positive or Negative) will be added to the dataframe in a new column called Sentiment.
The output of the project will be a CSV file with a header row that includes column names such as Title, Year, Synopsis, Review, Sentiment, and Original Language. The Original Language column will indicate the language of the review and synopsis (en/fr/sp) before translation. The dataframe will consist of 30 rows, with each row corresponding to a movie.

Tools used
Pandas: for data manipulation and analysis
HuggingFace Transformers: for natural language processing tasks, such as translation and sentiment analysis
PyTorch: for building and training machine learning models
Skills learned
Data cleaning and manipulation using Pandas
Natural language processing techniques, such as translation and sentiment analysis, using HuggingFace Transformers
Building and training machine learning models using PyTorch Integration of multiple tools and libraries to solve a complex problem
Overall, this project combines data manipulation, natural language processing, and machine learning techniques to perform multiple tasks on a dataset.

Project Rubric:
Fetch data
Criteria	Submission Requirements
Create a single dataframe by fetching data from the 3 CSV files. The dataframe should have the following columns -> ["Title", "Year", "Synopsis", "Review", and "Original Language"].

Students are able to create a Pandas dataframe of movie reviews by completing the preprocess_data() function.

Text Translation
Criteria	Submission Requirements
Load translation models and tokenizers from HuggingFace

Students are able to load the pretrained text translation models and tokenizers from HuggingFace.

Write a function to translate text using a model and a tokenizer (Complete translate())

Students are able to complete the translate() function.

Filter French and Spanish reviews and synopses in the dataframe and translate them to English.

Students should be able to use the translate() function to translate French and Spanish reviews and synopses to English and then update the dataframe.

Sentiment Analysis
Criteria	Submission Requirements
Analyze the sentiment of all the reviews in the dataframe using a pre-trained model from HuggingFace. Report sentiments as Negative/Positive by creating a new column called "Sentiment".

Students should load a sentiment analysis model, complete the function called analyze_sentiment, and then get the Sentiment (Negative, Positive) of all the movie reviews in the dataframe.
