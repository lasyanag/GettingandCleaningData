# Getting and Cleaning Data
How the script works
1. Merge the training and the test sets to create one data set 
- Combine the respective data in training and test data sets corresponding to subject, activity and features. The results are stored in subject, activity and features.
-The columns in the features data set can be named from the metadata in featureNames
- The data in features,activity and subject are merged and the complete data is now stored in completeData

2. Extracts only the measurements on the mean and standard deviation for each measurement
-Extract the column indices that have either mean or std in them.
-Add activity and subject columns to the list and look at the dimension of completeData
-Create extractedData with the selected columns in requiredColumns. And again, we look at the dimension of requiredColumns.

3. Uses descriptive activity names to name the activities in the data set 
-The activity field in extractedData is originally of numeric type. Change its type to character so that it can accept activity names. The activity names are taken from metadata activityLabels.
-Factor the activity variable, once the activity names are updated.

4. Appropriately labels the data set with descriptive variable names 
-Replace acronyms

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject
- First, set Subject as a factor variable.
-Create tidyData as a data set with average for each activity and subject. Then, we order the enties in tidyData and write it into data file Tidy.txt that contains the processed data.
