# Getting-and-Cleaning-Data-Assignment
## Introduction

This is the solution for the course project for the Getting and Cleaning Data located at https://class.coursera.org/getdata-013. 

The solution was completed on 4.26.2015 for the April 2015 class.

## Problem

<b>This section is a copy of the problem from the course assignment</b>


<i>The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project. You will be required to submit: 1) a tidy data set as described below, 2) a link to a Github repository with your script for performing the analysis, and 3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.  </i>

<i>One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: </i>

<i>http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones </i>

<i>Here are the data for the project: </i>

<i>https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip </i>

<i>You should create one R script called run_analysis.R that does the following. </i>

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement. 
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names. 
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

<i>Good luck!</i>


## Solution

### Files
|Files            |Description
|-----------------|----------------------------------------------|
|run_analysis.R   | Solution R code                              |
|output.txt       | output of the write.tables() call in step 5  |
|./UCI HAR Dataset| Input dataset defined by the problem         |

### Setup
The raw data is not downloaded with run_analysis.R from the repository, the raw data files must be placed in the original format in a directory named "UCI HAR Dataset" within the working directory.

### Usage
source (run_analysis.R)

### Output

* allData: The script creates a tidy data set with test and train data concatenated under allData.
* allDataMelt: contains the same results as allData, converted to a narrow dataset
* output: contains the tidy data set with the average of each variable for each activity and subject.



