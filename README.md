# Getting_Cleaning_Data
Getting and Cleaning Data Project

run_analysis.R processes raw data of UCI HAR Dataset to a new, clean, and tidy data set called "UCI_HAR_Dataset.txt"  

loading data:  
line 15 - 22: load data from raw data set to the following variables  
DT_test: test data set  
LB_test: activity labels of test set  
SB_test: subjects of test set  
DT_train: training data set  
LB_train: activity labels of training set
SB_train: subjects of training set
DT_feature: features of both test data set and training data set
Act_LB: descriptions of activity labels for test data set and training data set

cleaning and tyding data:
line 25: Match activity labels with activity names. Add activity names and subjects as new columns to test set.
line 26: Match activity labels with activity names. Add activity names and subjects as new columns to training set.
line 27: Merge test set and training set. Store the merged data set in DT_merge 
line 28: Rename the merged data set by replacing variables numbers with feature names.
line 29: Extract only the features regarding mean and std. Store the new data set in DT_merge_mean_std
line 30: Group the new data set by activity names and subjects with averaged values of features. Store the new data set in DT_new.
line 31: Output the clean data set to UCI_HAR_Dataset.txt.
