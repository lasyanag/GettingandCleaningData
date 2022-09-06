# Getting and Cleaning Data
How the script works
1. Merge the training and the test sets to create one data set We can use combine the respective data in training and test data sets corresponding to subject, activity and features. The results are stored in subject, activity and features.

2. Extracts only the measurements on the mean and standard deviation for each measurement

3. Uses descriptive activity names to name the activities in the data set The activity field in extractedData is originally of numeric type. We need to change its type to character so that it can accept activity names. The activity names are taken from metadata activityLabels.

4. Appropriately labels the data set with descriptive variable names Here are the names of the variables in extractedData

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject

