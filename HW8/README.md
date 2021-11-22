I worked alone on Homework 8. After downloading the Kaggle files, they came as zip files. 
I unziped them and stored them in a directory in my Google Drive called "DSPS2021/HiggsBoson." 
The kaggle.json file is stored in the directory DSPS2021/.kaggle, that is what I used for the 
kaggle authentication process. 

I then read in the data from the provided training set from training.csv.
I dropped the rows that had any -999.0 values in it as these were invalid data. This decision dropped 
a lot of the provided data, 250,000 entries to around 68,000 entries. 

There is one cell of code that must run for approximately <strong>30 minutes</strong>, for this I apologize. 
I was interested in seeing where the max depth of the regressors did not continue to have a better testing score, and made trees
with a max depth from 1 to 10. You can change the amount of max depths trials by changing the variable treeDepths
which is a list set initially to [1,2,3,4,5,6,7,8,9,10].


The Gradient Boosted Trees almost always out performed the Random Forest, however, the execution time for the Gradient Boosted Trees was 
quantitatively longer than the Random Forest. The regression models were not as effective in predicting as the classification models. This may have to do with the fact that
the regression models were predicting a continuous variable, while the classification models were predicting out of 3 types. 

-Jarod Dagney
jwdagney@udel.edu
