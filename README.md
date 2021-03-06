# Readme
This code creates the function "run_analysis", which takes data from the Human Activity Recognition Using Smartphones Data Set fom the UCI Machine Learning Repository (information on measurements and experiment available here: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones), and summarizes the mean and standard deviation measurements.

The original data consisted of 7 datasets, one training dataset, one test dataset, 2 datasets containing the subject ids for the test and training datasets, 2 datasets containing the activity ids for the training and test datasets, and one dataset containing the variables for each measurement. These were combined to create one data table containing 561 measurements for 30 subjects performing 6 activities a number of times and produce a table with a total of 10,299 instances. The function "run_analysis" first selects all mean and standard deviation measurements from the combined trainingg and and test datasets, creating a dataset with columns measuring 86 variables, and two variables indicating the subject and the activity being performed for each measurement. Data is then summarized by creating a mean score for each mean and standard deviation for each subject while performing each activity.

The table is then written to a text file named "Samsung_fitness_data.txt" (a blank .txt file the user should place in their working directory prior to running the function). 

The units for the measurements were measured by the original researchers as follows:

"The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

For each record it is provided:

- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment."



