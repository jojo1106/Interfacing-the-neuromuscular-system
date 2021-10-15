# EXERCISE 3

In this Exercise, an already decomposed EMG signal in the form of spike trains was used to reconstruct a synthetic original EMG signal from the motor unit spike trains. It was performed to understand the convolution of Motor Unit Action Potentials (MUAP) with spike trains, followed by an algebraic summation over all Motor Units action potentials to generate a modelled EMG signal that is similar to the original signal, but “clean” from noise and undetected motor units. After the subtraction of the reconstructed EMG signal from the original signal, the residual signal was obtained, in other words this corresponds to the noise and signals of undetected muscle fibre action potentials. 

### Task 1 Convolution Of MUAPT and spike trains

1)	Compute the Motor Unit Action Potentials for each motor unit using the Spike Triggered Average.

2)	Perform the convolution for each motor neuron and plot the results for all motor neurons in the same plot.

![convolution](https://user-images.githubusercontent.com/47339450/137549802-14611d41-ba23-4cb8-a815-3c77895a49e9.jpg)

![detailed_convolution](https://user-images.githubusercontent.com/47339450/137549830-28c2af67-468a-4744-9551-0be07dcdedbc.jpg)


### Task 2   Generation of EMG signal 
1)	To obtain the “clean” EMG signal, sum the convolutions obtained in task 1 and plot the result together with the original signal.  


![cleanVSoriginal](https://user-images.githubusercontent.com/47339450/137549896-f8642c7e-6ccd-4cb8-8487-efa4289307df.jpg)


### Task 3 Computing the residual signal
1)	Compute the residual EMG and plot it together with the clean and original signal.

![res_clean_orig](https://user-images.githubusercontent.com/47339450/137549933-15e67927-2ec3-4679-b6dc-4e4c5e11230b.jpg)


2)	Compute the correlations between all combinations of the 3 signals and explain the results.


![correlation](https://user-images.githubusercontent.com/47339450/137549954-17d937b0-81f3-4d2a-8857-a77a4b1c73b4.jpg)

![coherence](https://user-images.githubusercontent.com/47339450/137549979-e3a9b58c-1a65-4d73-8e06-bfae73559345.jpg)



