Through this assignment I try to use tf-idf metric to find which data to discard and which to keep in the result from the input
Using a test train 10-90 split, I try to find the best threshold to discard the data
Using tf-idf metric the idf value is calculated for each word in the training data and along with it the tf-idf score is calculated for each row in the training dataset
AFter calculating the tf-idf scores they are sorted and 50% tf-idf score is taken as a threshold(this can be easily changed to any other value)
The threshold is used to discard the data in the test dataset
If a row in test has a higher tf-idf score where the idf value used is from the value calculated from the training dataset then the row is kept in the result
If a row in test has a lower tf-idf score the row is discarded from the result
If the word is completely new the document frequency is taken as 1 increasing the idf score as the information is not redundant and we would like to keep it
Graphs are plotted for the tf-idf scores calculated for the training dataset and the test dataset to visualize the output as a evaluation measure for the threshold
As we can see none of the scores in the removed data are above the threshold and the scores in the kept data are above the threshold
