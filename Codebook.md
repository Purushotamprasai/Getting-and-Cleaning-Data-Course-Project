---
Title: CodeBook.md
output:
  word_document: default
  pdf_document: default
---

# About source data

The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project. You will be required to submit: 1) a tidy data set as described below, 2) a link to a Github repository with your script for performing the analysis, and 3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.

One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here are the data for the project:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip


#About R script

File with R code "run_analysis.R" does the following:

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set.
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

# Merging the training and the test sets to create one data set.

1. Loading and reading files
2. Loading and reading trainings tables
3. Loading and reading testing tables
4. Reading feature vector
5. Loading and Reading activity labels
6. Assigning column names
7. Merging all data in one set

# Extracting only the measurements on the mean and standard deviation for each measurement.

1. Reading column names
2. Create vector for defining ID, mean and standard deviation
3. Making nessesary subset from setAllInOne

# Using descriptive activity names to name the activities in the data set.

1. Appropriately labeling the data set with descriptive variable names
2. Creating a second, independent tidy data set with the average of each variable for each activity and each subject
3. Making second tidy data set
4. Writing second tidy data set in txt file

# About variables.

1. x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
2. x_data, y_data and subject_data merge the previous datasets to further analysis.
3.features contains the correct names for the x_data dataset, which are applied to the column names. 