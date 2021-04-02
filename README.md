# Sentiment-Analysis
### Sentiment Analysis using NLP
My project is based on the sentiment analysis of airline data set which consists of reviews given by passengers of the particular airline and our classes consists of 3 sentiments which are negative, positive and neutral.

I divided the project into 3 parts:

### 1.	Preprocessing the data
The textual data we receive from the csv file consists of filler words which are not useful for us and has to be removed otherwise they will hinder the process.

It consist of various sections:-

1.	**Tokenization** - It means converting our sentences into words so that they can be easily checked or compared for any updation or removal.

2.	**Removing Stopwords** - Removing stopwords is an important part of data preprocessing as these words are not useful and mainly disturbs our classifiers in choosing the import features as they dont have any meaning in the sentence like “the”,”I”,”has” etc.

3.	**Lemmatization/ Stemming** - The root form of the word can be generated from both lemmatization and stem but stem is capable of generating a word that isn’t present in the dictionary. We have considered Lemmatization as it is more commonly used than stemming.

### 2.	Vectorization 

After than we have a list of lemmatized words, now starts the main problem how can we find the most frequency words the prerequisite for this is that the list words should not have stopwords and punctuations so In our case we chose the TF-IDF VECTORIZER in this you can also apply things like if instead of single word as a training you can call 2, 3 words like “not good” which makes sense which can be done by n-grams methods and there are many functionalities which it can do.

TF-IDF stands for Term Frequency Inverse Document Frequency.It is a very good algorithm for transforming the words into frequencies which we can use to predict the outcome.

There are many algorithms instead of tf-idf like baggage count etc. but there is  more leniency in tf-idf.

After this our data is set to use in the classification models

### 3.	Using different classifiers

1. **SVM(Support Vector Machine)** - 
Gives accuracy of 76%

2. **Random Forest Classifier** -
Gives accuracy of 72%

3. **Multinomial Naive Bayes** -
Gives accuracy of 70%

4. **Naive Bayes(From Scratch)** -
Gives accuracy of 69%

5. **Combination of SVM and Multinomial Naive Bayes** -
Gives accuracy of 77%

### 4.	Results

- From this we can deduce that **SVM** works good for the data.
- Our Naive Bayes gives the almost same result as the Multinomial Naive Bayes
- Using ensemble learning we combined the result and got a better result.
- For this we have used 4000 tweets as the time taken to check the 11000 tweets is very much and takes around 45 minutes.
 


