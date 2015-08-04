# Coursera-Getting-and-Cleaning-Data
This file describes how run_analysis.R script works.

1.First, unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
  The unzip file will create a folder named "UCI HAR Dataset", make sure this folder and the run_analysis.R script are both in the current working directory.

2.Second, use source("run_analysis.R") command in RStudio.

3.Third, you will find two output files are generated in the current working directory:
  merged_data.txt (7.9 Mb): it contains a data frame called cleanedData with 10299*68 dimension.
  tidy_data.txt (220 Kb): it contains a data frame called result with 180*68 dimension.

4.Finally, use data <- read.table("tidy_data.txt") command in RStudio to read the file. Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.
