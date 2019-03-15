# text-classification
This repo contains text classification hands-on work for beginners in information retrieval.

**Feature	selection in the notebook**

| Model        | Implementation         |
| ------------- |-------------|
| BoW (Bag of Words model)	| Sklearn.CountVectorizer	Section|
| TF-IDF | Sklearn.CountVectorizer, Sklearn. TfidfTransformer	(With Naïve bayes) |
| Hashing Vectors	| Sklearn. HashingVectorizer |
| Hashing vectors along with Tf-idf | Sklearn. HashingVectorizer, Sklearn. TfidfTransformer |
| Dov2vec model	| gensim.models.doc2vec	|

**Claasifiers used in this work**

| Classifier        | Implementation         |
| ------------- |-------------|
| Naive Bayes | sklearn.naive_bayes.MultinomialNB |
| SVM |  sklearn.linear_model.SGDClassifier | 
| Random forest | sklearn.ensemble.RandomForestClassifier |
| Logistic regression | sklearn.linear_model.LogisticRegression | 


**Discussion**

*	SVM does better than the other classifiers as per the experiment. SVM with linear kernel is generally working well for high dimensional data and is faster to train. Among the features tried, SVM worked better with Tf-idf model.
*	Random forest did not achieve at least the accuracy given by the Naïve Bayes. This could be due dimensionality reduction (feature selection) happens inside random forest.
*	Random forest with default parameters took long time to train and test.
*	Naïve Bayes is also performs well in text classification as per the results and SVM does better than that.
*	Tf-idf performs better than Doc2vec. But this needs to be tested for multiple parameters before conclusion. Optimal parameter estimation technique like gridSearchCV is an option to do this.
*	HashingVector with Tf-idf trains really faster.
