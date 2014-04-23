Getting and Cleaning Data -- Coursera Course Project -- Completed by David Russell (Student)

==================================================================
Coursera Getting and Cleaning Data Course Project
==================================================================
Student: David Russell
==================================================================

The "run_analysis.R" script performs the following functions on the "Human Activity Recognition Using Smartphones Dataset -- Version 1.0", including:

1. Merges the training and the test sets to create one data set.

	-- A unique subject identifier variable was created based on the "subject_train.txt" and "subject_test.txt"  files provided with the original dataset. This subject identifier variable was named "subject_id".

	-- A unique activity identifier variable was created based on the "y_train.txt" and "y_test.txt" files provided with the original dataset. This activity identifier variable was named "activity_id". Textual descriptions of each     
	 activity are provided in the variable "activity"

	-- Mean and standard deviations for measurements in the Training and Test datasets were binded using the "rbind" 	   	   function in R 

2. Extracts only the measurements on the mean and standard deviation for each measurement. 

	-- For the purposes of this project, I have limited measurements to variables with labels containing the sub-strings "mean()", "meanFreq()", and "std()"

3. Uses descriptive activity names to name the activities in the data set

	-- Labels were assigned to each mean and standard deviation variable based on those listed in the "features.txt"         file
4. Appropriately labels the data set with descriptive activity names. 

	-- The "activity_id" variable corresponds to six activities with the following labels:

		1 WALKING
		2 WALKING_UPSTAIRS
		3 WALKING_DOWNSTAIRS
		4 SITTING
		5 STANDING
		6 LAYING

5. Creates a second, independent tidy data set with the average of each variable for each activity and each sbject. 

	-- The "run_analysis.R" script creates a tidy data set with the name "tidydata.txt"
