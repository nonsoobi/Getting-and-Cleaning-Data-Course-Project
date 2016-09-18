## Description

This contains additional information about the variables, data and transformations used in the Geting and Cleaning Data Course Project course project.

## Source Data

Full description of the data used in this project can be found [UCI Machine Learning repository](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

The source data for this project can be found [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)

## Data Set Information - Sourced from [UCI Machine Learning repository] (http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

## Attribute Information

For each record in the dataset it is provided:

Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
Triaxial Angular velocity from the gyroscope.
A 561-feature vector with time and frequency domain variables.
Its activity label.
An identifier of the subject who carried out the experiment.

#About variables:

x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
x_data, y_data and subject_data merge the previous datasets to further analysis.
features contains the correct names for the x_data dataset, which are applied to the column names stored in

## About R script

The "run_analysis.R" file, containing the R code, performs 5 following steps, according to the assigned task for the project:

### Section 1. Merge the training and the test sets to create one data set.
After setting the source directory for the files, read into tables the data located in 

<p>1.1 Reading files
<p>1.1.1 Reading trainings tables
<p>1.1.2 Reading testing tables
<p>1.1.3 Reading feature vector
<p>1.1.4 Reading activity labels
<p>1.2 Assigning column names
<p>1.3 Merging all data in one set

### Section 2. Extracting only the measurements on the mean and standard deviation for each measurement
<p>2.1 Reading column names
<p>2.2 Create a logical vector for defining ID, mean and standard deviation
<p>2.3 Making nessesary subset from setAllInOne

### Section 3. Using descriptive activity names to name the activities in the data set

### Section 4. Appropriately labeling the data set with descriptive variable names

### Section 5. Creating a second, independent tidy data set with the average of each variable for each activity and each subject
Per the project instructions, we need to produce only a data set with the average of each veriable for each activity and subject
<p> 5.1 Making second tidy data set
<p> 5.2 Writing second tidy data set in txt file

NOTE: The code takes for granted that all data is present in the same folder, un-compressed and without names altered.

