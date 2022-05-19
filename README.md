# PASCIR-dataset

Two versions were provided as part of the Physical Activities for Spinal Cord Injuries Rehabilitation (PASCIR) dataset. The first version provides segmented sensor data, which gives the researchers the ability to develop and evaluate their own algorithms. Table 1 shows the characteristics of the first version. The second version comprises a baseline feature set to allow researchers to focus on classifier development.      

# **Data Collection:** 

Data were collected using a single wireless sensor (Shimmer Research, Dublin, Ireland). It comprises a triaxial accelerometer with a sensitivity of 660 mV/g. Acceleration data was collected with a sampling frequency of 30 Hz (range ± 2 g). In terms of axis orientation, the Y-axis was parallel with the wrist, pointing toward the fingers and across the X-axis. Additionally, the Z-axis pointed away from the backside of the wrist.

Ten healthy individuals (three male, seven female; aged 29 ± 5.5 years) were asked to perform a series of physical activities performed during the rehabilitation of spinal cord injuries, including shoulder abduction (SA), elbow extension (EE), elbow flexion (EF), shoulder external rotation (SER), shoulder internal rotation (SIR), shoulder extension (SE), and shoulder flexion (SF) 

  **Table 1: Characteristics of the first version of the PASCIR dataset.**

![image](https://user-images.githubusercontent.com/105864750/169359581-3ae963b5-8487-4483-93a9-3ef13d1be59a.png)

# **Data Format:**

In the first version, data are stored in seven separate files, where each file consists of data from one subject performing one type of activity. Thus, there are seven files associated with each subject. The accelerometer measurement is recorded on a separate line in the data file with the following format: <timestamp, x, y, z, activity >. The timestamp is the time at which the sensor value was recorded, the x, y, and z values represent the sensor values for the x, y, and z spatial axes, respectively, and the activity label identifies the physical activity. 

In the second version, the baseline feature set is recorded on a separate line in the data file. Each line consists of the corresponding activity label, subject id, and the values of features extracted from the three axes (x, y, and z) of the acceleration data and the signal magnitude (m). The list of features used includes minimum, maximum, range, mean, standard deviation, and root mean square. This version has 700 samples, with each activity represented by 100 samples.
