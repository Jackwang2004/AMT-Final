The Sentiment Analysis file contains the contents when I tried to train on Amazon's video game review dataset that has ratings highly concentrated on the higher end (in fact, we find that over 50% of people give a 5). But, with a test set divided evenly between reviews with ratings of 5 and reviews without, the model produced exactly 50% accuracy, indicating overfitting to the abundance of positive reviews in the training set. 

The Sentiment Analysis FINAL file attempts to resolve this problem by creating a training set that, like the test set, contains an equal number of reviews that are positive or negative, using the threshold value POSITIVE set by the user. This led to more promising results. 

More explanation of the program is given as comments in the files themselves, along with frequent debug/testing checks for each part of the code. 

To run this program, you need to download the Amazon Video Game review JSON file at the "5-core" section here: https://jmcauley.ucsd.edu/data/amazon/

Keep in mind that although the collective size of the training and test set is adjustable, because Sentiment Analysis FINAL makes training and testing sets with an equal number of positive and negative reviews, the actual maximum SIZE is lower than the 230k reviews in the JSON file and depends on the POSITIVE threshold selected. 
