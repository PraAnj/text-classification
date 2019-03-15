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
