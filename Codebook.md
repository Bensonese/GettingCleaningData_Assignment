### Code Book for the data set file "assignment_tidy_data.txt"

#### The data set includes the following variables:

##### [1] "Subject"                       

##### [2] "Activity"

##### [3-68] Measurement data (please see below for a complete list of these 66 variable names) 

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

"Time_BodyAcc_mean_X"           "Time_BodyAcc_mean_Y"           "Time_BodyAcc_mean_Z"          
"Time_BodyAcc_std_X"            "Time_BodyAcc_std_Y"            "Time_BodyAcc_std_Z"           
"Time_GravityAcc_mean_X"        "Time_GravityAcc_mean_Y"        "Time_GravityAcc_mean_Z"       
"Time_GravityAcc_std_X"         "Time_GravityAcc_std_Y"         "Time_GravityAcc_std_Z"        
"Time_BodyAccJerk_mean_X"       "Time_BodyAccJerk_mean_Y"       "Time_BodyAccJerk_mean_Z"      
[16] "Time_BodyAccJerk_std_X"        "Time_BodyAccJerk_std_Y"        "Time_BodyAccJerk_std_Z"       
[19] "Time_BodyGyro_mean_X"          "Time_BodyGyro_mean_Y"          "Time_BodyGyro_mean_Z"         
[22] "Time_BodyGyro_std_X"           "Time_BodyGyro_std_Y"           "Time_BodyGyro_std_Z"          
[25] "Time_BodyGyroJerk_mean_X"      "Time_BodyGyroJerk_mean_Y"      "Time_BodyGyroJerk_mean_Z"     
[28] "Time_BodyGyroJerk_std_X"       "Time_BodyGyroJerk_std_Y"       "Time_BodyGyroJerk_std_Z"      
[31] "Time_BodyAccMag_mean"          "Time_BodyAccMag_std"           "Time_GravityAccMag_mean"      
[34] "Time_GravityAccMag_std"        "Time_BodyAccJerkMag_mean"      "Time_BodyAccJerkMag_std"      
[37] "Time_BodyGyroMag_mean"         "Time_BodyGyroMag_std"          "Time_BodyGyroJerkMag_mean"    
[40] "Time_BodyGyroJerkMag_std"      "Freq_BodyAcc_mean_X"           "Freq_BodyAcc_mean_Y"          
[43] "Freq_BodyAcc_mean_Z"           "Freq_BodyAcc_std_X"            "Freq_BodyAcc_std_Y"           
[46] "Freq_BodyAcc_std_Z"            "Freq_BodyAccJerk_mean_X"       "Freq_BodyAccJerk_mean_Y"      
[49] "Freq_BodyAccJerk_mean_Z"       "Freq_BodyAccJerk_std_X"        "Freq_BodyAccJerk_std_Y"       
[52] "Freq_BodyAccJerk_std_Z"        "Freq_BodyGyro_mean_X"          "Freq_BodyGyro_mean_Y"         
[55] "Freq_BodyGyro_mean_Z"          "Freq_BodyGyro_std_X"           "Freq_BodyGyro_std_Y"          
[58] "Freq_BodyGyro_std_Z"           "Freq_BodyAccMag_mean"          "Freq_BodyAccMag_std"          
[61] "Freq_BodyBodyAccJerkMag_mean"  "Freq_BodyBodyAccJerkMag_std"   "Freq_BodyBodyGyroMag_mean"    
[64] "Freq_BodyBodyGyroMag_std"      "Freq_BodyBodyGyroJerkMag_mean" "Freq_BodyBodyGyroJerkMag_std" 