# Code Book

### Variables:
features: The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ
activities: List of activities performed when the corresponding measurements were taken and its codes
subject_test: contains test data of 9/30 volunteer test subjects being observed
x_test: contains recorded features test data
y_test: contains test data of activities’code labels
subject_train: contains train data of 21/30 volunteer subjects being observed
x_train: contains recorded features train data
y_train: contains train data of activities’code labels
X: Is made by binding the x_train and x_test data
Y: Is made by binding the y_train and y_test data
Subject: Is made by binding the subject_train and subject_test data
Merged_Data: Is made by binding the X, Y, and Subject data
TidyData: Is created by subsetting Merged_Data, selecting only columns: subject, code and the measurements on the mean and std
for each measurement

### For Step 3:
Entire numbers in code column of the TidyData replaced with corresponding activity taken from second column of the activities variable

### Step 4:
code column in TidyData renamed into activities
All Acc in column’s name replaced by Accelerometer
All Gyro in column’s name replaced by Gyroscope
All BodyBody in column’s name replaced by Body
All Mag in column’s name replaced by Magnitude
All start with character f in column’s name replaced by Frequency
All start with character t in column’s name replaced by Time

### Step 5:
FinalData is created by sumarizing TidyData taking the means of each variable for each activity and each subject, after groupped by subject and activity.
Export FinalData into FinalData.txt file.
