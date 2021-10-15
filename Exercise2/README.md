# EXERCISE 2

The purpose of this exercise is to understand the general purposes of surface EMG decomposition and analysis of motor unit spike trains. You will learn how to perform spike triggered averaging and coherence analysis. These exercises will teach you how to analyse spike trains (series of delta functions with zeros and ones) that correspond to the action potential sent by individual neurons. 
Please do not hesitate to ask questions on the StudOn forum regarding the tasks or activating the Campus-Wide License for MATLAB. We also encourage you to post your results to the respective thread in the forum. Don’t forget to label your axes whenever you plot a graph and to discuss what you see.

### Task 1 – All-or-none response

The names of the variables from the file that you will use for this exercise are SIG, MUPulses and fsamp, corresponding to the EMG channel data, the motor unit impulses and sampling rate. MUPulses is a cell array where each cell corresponds to the firing instances of one neuron (in this case a motor unit). This number is stored in samples, therefore, MUPulses{1}(1) is the first firing of neuron #1. 
In this first task, you will compute the binary code corresponding to firings of each motor unit. 
As you may already know, neurons work according to the all-or-none principle; the binary code is a vector which has the same length as the EMG signal with each motor unit having entries with ones and zeros (1 - firing, 0 - no firing).

1)	Convert each MUPulses into a binary code. The result is a matrix with rows equal to the number of neurons and with columns equal to the length of the task (the EMG signal length, that you can take from the first EMG channel - e.g. length (EMG(1,:)). 

### Task 2 Average an estimate of the Neural Drive to the muscle
 
1)	Compute the cumulative spike train (CST) which is the sum of these binary codes for all motor units.

... TODO Bild


2)	Compute the average number discharge rate per second (firings/second) by dividing CST with the number of active motor units with a moving average window (as you have done with the RMS in the previous practical exercise). Use 50, 100, and 200 ms windows.

... TODO Bild 

### Task 3 Spike triggered average

Spike triggered averaging is a useful event detection tool that is often used in neural signal processing. The aim is to investigate the temporal relation between a spike train and a continuous signal (EMG in this case) in order to reveal the response in electrophysiological activity preceding a spike. To compute the STA,
1)	For each spike round to the nearest integer a time window that is centred at the spike and holds values from (-X to: +X) with X being 100, 50, 25, and 15 milliseconds. 
2)	Compute this average for all set of electrodes and plot the motor unit action potential waveform.

... TODO Bild

### Task 4 Coherence

Coherence analysis is a bounded measure of the linear association between two signals in the frequency domain. Therefore, it is very useful for estimating the common synaptic input of a pair of motor units.

1) Compute the coherence between two increasing size of motor units and plot the result. (Hint: look at the MATLAB documentation to find how to use the mscohere function) 

... TODO Bild 

