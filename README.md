# gettingandcleaning
# Getting and Cleaning Data - Course Project

This project is part of the "Getting and Cleaning Data" course on Coursera.

## Objective

The goal of this project is to demonstrate the ability to collect, work with, and clean a data set. The final output is a tidy data set that can be used for further analysis.

## Dataset

The data used in this project comes from the [Human Activity Recognition Using Smartphones Dataset](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones), which contains accelerometer and gyroscope data collected from a Samsung Galaxy S smartphone.

## Files in the Repository

- `run_analysis.R`: R script that processes the raw data and creates the tidy dataset.
- `TidyData.txt`: Final tidy data set with the average of each variable for each activity and each subject.
- `CodeBook.md`: Describes the variables in the data and the transformations performed.
- `README.md`: Explanation of the project and how the files are connected.

## How the Script Works

1. Downloads and unzips the dataset.
2. Reads training and test data sets.
3. Merges them into one data set.
4. Extracts only the measurements on the mean and standard deviation.
5. Uses descriptive activity names.
6. Appropriately labels the data set with descriptive variable names.
7. Creates a second tidy data set with the average of each variable for each activity and each subject.
8. Writes the tidy data set to `TidyData.txt`.

## Required Libraries

- `dplyr`

## How to Run

Place `run_analysis.R` in your R working directory and run the script. It will generate a file called `TidyData.txt`.
