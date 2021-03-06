# About the source data

The source data are from the Human Activity Recognition Using Smartphones Data Set. 

A full description is available at the site where the data was obtained: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

Here are the data for the project: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip


# About run_analysis.R

File with R code "run_analysis.R" performs the 5 following steps (in accordance assigned task of course work):

- Reading in the files and merging the training and the test sets to create one data set.
  - Reading files
    - Reading trainings tables
    - Reading testing tables
    - Reading feature vector
    - Reading activity labels
  - Assigning variable names
  - Merging all data in one set
- Extracting only the measurements on the mean and standard deviation for each measurement
  - Reading variable names
  - Create vector for defining ID, mean and standard deviation
  - Making nessesary subset from merged data set
- Using descriptive activity names to name the activities in the data set
- Appropriately labeling the data set with descriptive variable names
- Creating a second, independent tidy data set with the average of each variable for each activity and each subject
  - Making second tidy data set
  - Writing second tidy data set in txt file

# About variables

- `x_train`, `y_train`, `x_test`, `y_test`, `sub_train` and `sub_test` contain the data from the downloaded files.
- `x_total`, `y_total` and `sub_total` merge the previous datasets to further analysis.
- `sel_features` contains the correct names for the `x_total` dataset, which are applied to the column names stored in
