# Information
Further details on Experiment and Dataset information can be found here
[Human Activity Recognition Using Smartphones Data Set](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones#)

# Variables from datasets
* activity - the six activities performed by subjects 
    * (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING)
* subject - a group of 30 volunteers within an age bracket of 19-48 years that participated in experiment

# Process of Data Clean Up
1. Data is downloaded from the following link and extracted to local computer:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
    * activity_lables.txt
    * features.txt
    * subject_train.txt
    * subject_test.txt
    * X_train.txt
    * X_test.txt
    * y_train.txt
    * y_test.txt
2. The training and the test sets are merged to create one data set.
3. The merged data set is reduced by extracting only the measurements on the mean and standard deviation for each measurement.
4. Descriptive activity names are used to name the activities in the data set are added based on what's listed from the activity_lables.txt file
5. Appropriately label the data set with descriptive variable names by altering the column headers
6. Lastly, with the the data set in step 4, the script will create a second, independent tidy data set with the average of each variable for each activity and each subject. This will be saved on local computer as <b>TidyData.txt</b>
