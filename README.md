# ECE-GY-6143_Project
This is the GitHub repository for the project in ECE-GY-6143 *Introduction to Machine Learning* course.



## Group Members

| Group Member   | NYU NetID |
| -------------- | --------- |
| Jielong Tang   | jt3994    |
| Xiaotian Zhou  | xz2850    |
| Zhaoxiong Chen | zc1728    |



## About Project

In this project, we plan to use traditional machine learning (ML) algorithm and deep learning (neural network) to train a film emotion classification model through the semantic recognition of film reviews. At the same time, different preprocessing is adopted for this data set to generate word vectors with larger information entropy.



## About Dataset

This project is based on Cornell Movie Review Data, available [here](https://www.cs.cornell.edu/people/pabo/movie-review-data). 

The data set is about the emotional classification of movies reviews, which includes 5331 positive snippets and 5331 negative snippets.

This data was first used in Bo Pang and Lillian Lee's paper in 2005.  \[1\]\[2\]



## Performance Comparison

So far, we have implemented Long Short-term Memory (LSTM), Naive Bayes (NB) and Support Vector Machine (SVM). The performance are provided in the following table.

| Model | Best Performance | Configuration |
| ----- | ---------------- | ---- |
| LSTM  | 76.24% |Epochs = 2000<br />Batch Size = 64|
| NB    | 76.20% |Feature selected based on information gain<br />Multinomial Naive Bayes model|
| SVM   | 69.59% |Feature selected based on frequency<br />Regularization C = 1|

According to Yoon Kim's paper, Convolutional Neural Network (CNN) could also be applied to movie emotion classification. Here is the performance of CNN from the paper. \[3\]

| Model | Best Performance | Configuration |
| ----- | ---------------- | ---- |
| CNN   | 81.50% |CNN-non-static model|



## Future Work

1. Consider using word2vec as word vectors.
   Since word2vec is a word vectorization model that supported well by the machine learning community. It is believed that using word2vec can help us achieve better performance.
2. Design more deep neural network (DNN) training models in emotion classification.
   Apart from training image data, lots of DNN models can also be employed in natural language processing region.



## Reference

[1] B. Pang and L. Lee, "Seeing Stars: Exploiting Class Relationships for Sentiment Categorization with Respect to Rating Scales," *Proceedings of the 43rd Annual Meeting of the Association for Computational Linguistics,* pp. 115-124, June 2005.

[2] B. Pang, L. Lee and S. Vaithyanathan, "Thumbs up? Sentiment Classification using Machine Learning Techniques," *Proceedings of the 2002 Conference on Empirical Methods in Natural Language Processing,* pp. 79-86, July 2002.

[3] Y. Kim, "Convolutional Neural Networks for Sentence Classiﬁcation," *Proceedings of the 2014 Conference on Empirical Methods in Natural Language Processing,* pp. 1746--1751, October 2014.

[4] E. Dapšauskas, "Movie Review Sentiment Polarity Classifier," 15 August 2019. [Online]. Available: https://github.com/Elijas/movie-review-sentiment-polarity-classifier. [Accessed 1 November 2020].

[5] C. Masch,  "Text classification with Convolution Neural Networks (CNN)," 15  December 2019. [Online]. Available:  https://github.com/cmasch/cnn-text-classification. [Accessed 1 November  2020].

[6] Pablov, "Spam classification with Naive Bayes and Support Vector Machines.," 2017. [Online]. Available: https://www.kaggle.com/pablovargas/naive-bayes-svm-spam-filtering. [Accessed 1 December 2020].