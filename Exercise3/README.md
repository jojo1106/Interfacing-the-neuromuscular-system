# EXERCISE 3

In this Exercise, you will work with an already decomposed EMG signal in the form of spike trains and you will need to reconstruct a synthetic original EMG signal from the motor unit spike trains. You will understand the convolution of Motor Unit Action Potentials (MUAP) with spike trains, followed by an algebraic summation over all Motor Units action potentials to generate a modelled EMG signal that is similar to the original signal, but “clean” from noise and undetected motor units. See the scheme below for an idea of the workflow and mathematical expression. After the subtraction of the reconstructed EMG signal from the original signal, we obtain the residual signal, in other words this corresponds to the noise and signals of undetected muscle fibre action potentials. 

### Task 1 Convolution Of MUAPT and spike trains
1)	Compute the Motor Unit Action Potentials for each motor unit using the Spike Triggered Average. See Exercise 2 if you need a reminder on the STA. 
To generate the original EMG signal, we need to convolute the spike train (array of zeros and ones) with the corresponding MUAPT for each motor neuron. Check the documentation for the MATLAB function conv() for the next step.
2)	Perform the convolution for each motor neuron and plot the results for all motor neurons in the same plot.


... TODO Bild

### Task 2   Generation of EMG signal 
1)	To obtain the “clean” EMG signal, sum the convolutions obtained in task 1 and plot the result together with the original signal. Note that you have to perform this for all channels of the EMG grid with the corresponding MUAP. 


... TODO Bild

### Task 3 Computing the residual signal
1)	Compute the residual EMG and plot it together with the clean and original signal.

... TODO Bild

2)	Compute the correlations between all combinations of the 3 signals and explain the results.

... TODO Bild

