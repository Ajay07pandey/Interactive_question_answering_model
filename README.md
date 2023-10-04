# Interactive_question_answering_model
 Wikipedia article Question answering data set 


There are three question files, one for each year namely S08, S09, and S10

The "question_answer_pairs.txt" files contain both the questions and answers. The columns in this file are as follows:

ArticleTitle is the name of the Wikipedia article from which questions and answers initially came.

1. ArticleTitle	
2. Question
3. Answer	
4. DifficultyFromQuestioner
5. DifficultyFromAnswerer	
6. ArticleFile

But we are only interested in question-answer features so we are taking them only.
Done the Following steps:
1. Merging all the dataset to One
2. Removing Duplicate Questions and Values From Data set
3. Removing Null Values
4. Prepared the Data set For NLP by
   * Removing Punctuation.
   * Removing Stopwords and removing White spaces.
   * Text Tokenization
   * Text Normalization
   * Text Vectorization Using Tfidf Vectorizer.
5. Model Implementation Using Cosine Similarity Matrix:
   
   Function -- ask('What does the "voice" of a violin depend upon?')
   
   Output:-
   
             Closest question found: what doe the voice of a violin depend upon
   
             Similarity: 97.19%
   
             Answer: shape
   
7. Model Using Python Threads and Levenshtein distance.

   Eg:-
   
           str1 = 'What does the of a violin depend upon?'
   
           str2 = most_similar_question.
   
           Function -- levenshtein_distance(str1, str2)
   
           Output -- Levenshtein distance is: 9

