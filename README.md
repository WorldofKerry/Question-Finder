# open-book-mc-tool
Matches a given question to the most similar questions in a question pool. 

## Usage
Create a `questions.csv` in the form of question, answer, [choice1], [choice2], [choice3], with the ones in [] being optional. 
Then when you run `main()` after re-loading the csv, it will prompt you for a question, fill it in, press enter, and it'll give you the most similar questions in your `questions.csv`.

## Stack
Uses sklearn's TfidfVectorizer under feature extraction for text, with nltk.corpus' stopwords to preprocess text. 
