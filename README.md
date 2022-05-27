# Classification-of-cased-and-uncased-in-text-classification-using-BERT

**ANUHYA KALVAKALA**

Here we are doing fine tuning for Bert model for text classification. Where we are considering a Bert cased vs uncased models in which we used distilbert-base-uncased and dilstilbert-base-uncased.

Here the main difference between cased and uncased is that training using case of text in word piece tokenization step and presence of accent makers.

In the Uncased models the text will be lower cased before it is word piece tokenized and if any accent is used that also will be removed.

In cased models the text will not be changed before it is word piece tokenized and accent is preserved.

In most of the cases Bert uncased will be more efficient but during POS tagging Cased plays a major role.

Below are the outputs of the data with their accuracies for the acllmb data given for the two models.

**distilbert-base-uncased**

We have used the distilbert base uncased to our dataset where we found the accuracy after training and testing data is 84.9%. Where CLS and SEP token ids are mentioned as 101 and 102

Accuracy on test data: **0.8495000004768372**

**distilbert-base-cased**

We have used the distilbert base cased to our dataset where we found the accuracy after training and testing data is 81.1%. Where CLS and SEP token ids are mentioned as 101 and 102 

Accuracy on test data: **0.8115000128746033**

**SELF TEST DATA**

Below are the results of the own test data on the two Bert models trained acllmbd  data and tested on own data where positive 13 and negative 13 comments are sent in one file of each for negative and positive reviews
For the distilbert cased data we tried to test the data on the model we trained using accllmb data and got an accuracy of 50% once and 100% once when testing it several times.

**CASED with test data**

Accuracy on test data: **0.5199999809265137**

**Uncased with test data**

Below is the result for the uncased distilbert data which we testing against the trained model using accllmb data and got an accuracy of 52% for the test data and prediction values for [pos,neg]

Accuracy on test data: **0.5199999809265137**

The own data has been tested and trained again and output results achieved are same as the test data achieved runed against the trained one accllmb data.




