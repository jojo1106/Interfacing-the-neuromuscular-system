# EXERCISE 2

The purpose of this exercise is to understand the general purposes of surface EMG decomposition and analysis of motor unit spike trains. It was taught how to perform spike triggered averaging and coherence analysis. These exercises teached how to analyse spike trains (series of delta functions with zeros and ones) that correspond to the action potential sent by individual neurons. 

### Task 1 – All-or-none response
 
Compute the binary code corresponding to firings of each motor unit. 

1)	Convert each MUPulses into a binary code. The result is a matrix with rows equal to the number of neurons and with columns equal to the length of the task (the EMG signal length, that you can take from the first EMG channel). 

### Task 2 Average an estimate of the Neural Drive to the muscle
 
1)	Compute the cumulative spike train (CST) which is the sum of these binary codes for all motor units.

![cst](https://user-images.githubusercontent.com/47339450/137546708-d1f4dd5f-47b2-4c2c-b495-546c4e00b022.jpg)


2)	Compute the average number discharge rate per second (firings/second) by dividing CST with the number of active motor units with a moving average window (as you have done with the RMS in the previous practical exercise). Use 50, 100, and 200 ms windows.


![Average_discharge](https://user-images.githubusercontent.com/47339450/137546736-763f5559-79f9-4a3e-bb44-c01201624ff8.jpg)


### Task 3 Spike triggered average

Spike triggered averaging is a useful event detection tool that is often used in neural signal processing. The aim is to investigate the temporal relation between a spike train and a continuous signal (EMG in this case) in order to reveal the response in electrophysiological activity preceding a spike. To compute the STA,
1)	For each spike round to the nearest integer a time window that is centred at the spike and holds values from (-X to: +X) with X being 100, 50, 25, and 15 milliseconds. 
2)	Compute this average for all set of electrodes and plot the motor unit action potential waveform.

![STA](https://user-images.githubusercontent.com/47339450/137546788-b9591970-e66a-4148-86db-682d54c06136.jpg)


### Task 4 Coherence

Coherence analysis is a bounded measure of the linear association between two signals in the frequency domain. Therefore, it is very useful for estimating the common synaptic input of a pair of motor units.

1) Compute the coherence between two increasing size of motor units and plot the result. (Hint: look at the MATLAB documentation to find how to use the mscohere function) 

![Coherence_hamming](https://user-images.githubusercontent.com/47339450/137546859-a5da3ff4-a587-4761-9e91-b92acb59c53c.jpg)

