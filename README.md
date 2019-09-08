## HumanActivityRecognition


This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying.

This dataset is collected from 30 persons(referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.

## How data was recorded
By using the sensors(Gyroscope and accelerometer) in a smartphone, they have captured '3-axial linear acceleration'(tAcc-XYZ) from accelerometer and '3-axial angular velocity' (tGyro-XYZ) from Gyroscope with several variations.

## Quick overview of the dataset :
Accelerometer and Gyroscope readings are taken from 30 volunteers(referred as subjects) while performing the following 6 Activities.

Walking
WalkingUpstairs
WalkingDownstairs
Standing
Sitting
Lying.
•	Readings are divided into a window of 2.56 seconds with 50% overlapping.

•	Accelerometer readings are divided into gravity acceleration and body acceleration readings, which has x,y and z components each.

•	Gyroscope readings are the measure of angular velocities which has x,y and z components.

•	Jerk signals are calculated for BodyAcceleration readings.

•	Fourier Transforms are made on the above time readings to obtain frequency readings.

•	Now, on all the base signal readings., mean, max, mad, sma, arcoefficient, engerybands,entropy etc., are calculated for each window.

•	We get a feature vector of 561 features and these features are given in the dataset.

•	Each window of readings is a datapoint of 561 features.



## How data set is working for deep learning

•	Here the time series data is divided in to several windows
•	At that window consider what is the accrelometer X,Y,Z axis signals and what is gyroscope X,Y,Z signals and what task is performed by the invidule at the current window
•	Considering these information several windows are created with the respective output class
•	take all the windows for all the 21 person (as discussed 70% of data train data) as train data
•	take all the windows for data of 7 person as test


## Authors
•	B ASUTOSH- Complete work  

## Acknowledgments
•	Applied AI Course
