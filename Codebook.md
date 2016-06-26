### Code Book for the data set file "assignment_tidy_data.txt"

#### The data set includes the following variables:

##### [1] "Subject"

The ID of the subject who performed the activity for each sample. Its range is from 1 to 30.

##### [2] "Activity"

The type of activity the subject was performing when the measurement was taken. There are six alternatives: 'Laying', 'Sitting',  'Standing', 'Walk Upstairs', 'Walking', 'Walking Downstairs'. 

##### [3-68] Measurement data (see below for a complete list of these 66 variable names) 

These data came from the accelerometer and gyroscope 3-axial raw signals Time_Acc_XYZ and Time_Gyro_XYZ. These time domain signals (denoted by prefix 'Time_') were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (Time_BodyAcc_XYZ and Time_GravityAcc_XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (Time_BodyAccJerk_XYZ and Time_BodyGyroJerk_XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (Time_BodyAccMag, Time_GravityAccMag, Time_BodyAccJerkMag, Time_BodyGyroMag, Time_BodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing Freq_BodyAcc_XYZ, Freq_BodyAccJerk_XYZ, Freq_BodyGyro_XYZ, Freq_BodyAccJerkMag, Freq_BodyGyroMag, Freq_BodyGyroJerkMag. (Note the 'Freq_' prefex denotes frequency domain signals). 

###### Additional notes: 

* Values are normalized and bounded within [-1,1].
* mean: Mean value
* std: Standard deviation
* The values in the tidy data set consist of averaged measurement data for each subject during each activity.
* '_XYZ' is used to denote 3-axial signals in the X, Y, and Z directions.

"Time_BodyAcc_mean_X"           "Time_BodyAcc_mean_Y"           "Time_BodyAcc_mean_Z"          
"Time_BodyAcc_std_X"            "Time_BodyAcc_std_Y"            "Time_BodyAcc_std_Z"           
"Time_GravityAcc_mean_X"        "Time_GravityAcc_mean_Y"        "Time_GravityAcc_mean_Z"       
"Time_GravityAcc_std_X"         "Time_GravityAcc_std_Y"         "Time_GravityAcc_std_Z"        
"Time_BodyAccJerk_mean_X"       "Time_BodyAccJerk_mean_Y"       "Time_BodyAccJerk_mean_Z"      
"Time_BodyAccJerk_std_X"        "Time_BodyAccJerk_std_Y"        "Time_BodyAccJerk_std_Z"       
"Time_BodyGyro_mean_X"          "Time_BodyGyro_mean_Y"          "Time_BodyGyro_mean_Z"         
"Time_BodyGyro_std_X"           "Time_BodyGyro_std_Y"           "Time_BodyGyro_std_Z"          
"Time_BodyGyroJerk_mean_X"      "Time_BodyGyroJerk_mean_Y"      "Time_BodyGyroJerk_mean_Z"     
"Time_BodyGyroJerk_std_X"       "Time_BodyGyroJerk_std_Y"       "Time_BodyGyroJerk_std_Z"      
"Time_BodyAccMag_mean"          "Time_BodyAccMag_std"           "Time_GravityAccMag_mean"      
"Time_GravityAccMag_std"        "Time_BodyAccJerkMag_mean"      "Time_BodyAccJerkMag_std"      
"Time_BodyGyroMag_mean"         "Time_BodyGyroMag_std"          "Time_BodyGyroJerkMag_mean"    
"Time_BodyGyroJerkMag_std"      "Freq_BodyAcc_mean_X"           "Freq_BodyAcc_mean_Y"          
"Freq_BodyAcc_mean_Z"           "Freq_BodyAcc_std_X"            "Freq_BodyAcc_std_Y"           
"Freq_BodyAcc_std_Z"            "Freq_BodyAccJerk_mean_X"       "Freq_BodyAccJerk_mean_Y"      
"Freq_BodyAccJerk_mean_Z"       "Freq_BodyAccJerk_std_X"        "Freq_BodyAccJerk_std_Y"       
"Freq_BodyAccJerk_std_Z"        "Freq_BodyGyro_mean_X"          "Freq_BodyGyro_mean_Y"         
"Freq_BodyGyro_mean_Z"          "Freq_BodyGyro_std_X"           "Freq_BodyGyro_std_Y"          
"Freq_BodyGyro_std_Z"           "Freq_BodyAccMag_mean"          "Freq_BodyAccMag_std"          
"Freq_BodyBodyAccJerkMag_mean"  "Freq_BodyBodyAccJerkMag_std"   "Freq_BodyBodyGyroMag_mean"    
"Freq_BodyBodyGyroMag_std"      "Freq_BodyBodyGyroJerkMag_mean" "Freq_BodyBodyGyroJerkMag_std" 
