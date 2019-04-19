# NBCMovieReviews
Machine Learning Project to classify movie reviews as positive or negative, Naive Bayes from scratch.

There are two folders (i.e., training data and test data), each of which includes a folder of positive reviews and a folder of negative reviews.
All the reviews in the positive review folders are labeled as 1, whereas the reviews in the negative review folders are labeled as 0.
The goal is to implement and train a Naive Bayes classifier from scratch to predict whether a review in the test data is +ve or -ve

I used the bag-of-words model and the number of occurrence of words in each review as its feature.
It is assumed the positions of words do not matter and each attribute value is independently generated. 
In case a word in the test data has not been seen in the training data, Laplace (add-1) smoothing for Naive Bayes is used.

Create two dictionaries one for positive and one for negative, each will keep the count of appeareance of a word.
CountDocs, keep the track of total number of reviews per class.
CountTerms, keep track of total number of words in a dictionary.
Open reviews and count the occurences of words in each review add it to total frequency of each word.
Calculate the likelyhood of a word given reviews class
Open testing reviews and predict the class for each review.

