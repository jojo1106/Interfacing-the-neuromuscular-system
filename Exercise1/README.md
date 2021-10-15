EXERCISE 1

Introduction

The purpose of this exercise is to practise the very basics of signal processing and analysis with MATLAB. We will use MATLAB functions to visualize, quantify and try to make sense of the EMG signal. If you have never programmed with MATLAB before, you can watch the tutorial lecture uploaded on StudOn. If you don’t have the license yet, click on the link below and take advantage of FAU’s Campus-Wide License to install and use MATLAB on your computer:
www.mathworks.com/products/matlab/student.html
Please don’t hesitate to ask questions on the StudOn forum regarding the tasks or activating the Campus-Wide License. We also encourage you to post your plots to the respective thread in the forum. Don’t forget to label your axes and to specify the task number associated with the plot. 

Task 1

MAT files are binary MATLAB files that store workspace variables. By loading the saved files to your MATLAB workspace, you get access to manipulate or visualize the variables. The names of the variables from the file that you will use for this exercise are SIG and ref_signal, fsamp corresponding to the EMG channel data and the force signal, respectively.
1)	Load the EMG file
2)	Plot each channel


..... TODO Bild

Task 2

Root-Mean-Square (RMS) of an EMG signal is calculated over a period of time and it is the square root of the average power of the signal. In other words, the negative voltage values are made positive since the signal is rectified. The reason why the RMS is used as a measure to quantify the EMG signal is that it reflects the physiological activity during contraction.
1)	Compute and plot the RMS in different time window lengths (50ms, 100ms, 200ms, 300ms, 400ms, 500ms) for each channel

.... TODO Bild

Task 3

In signal analysis, it is common to look for linear correlations where a change in one variable corresponds to a directly proportional change in another variable. The correlation coefficient r determines how strong the correlation is. The value of r ranges from -1 to 1, where -1 shows a perfect negative correlation and 1 shows a perfect positive correlation. A correlation coefficient value of 0 means there is no linear relationship between the variables.
1)	Correlate the average signal taken at 50ms and 200ms with force, i.e. compute the correlation coefficient r

... TODO Bild

2)	Plot the correlation (force as a function of EMG), and find which window length correlates better and explain why. 


.... TODO Bild