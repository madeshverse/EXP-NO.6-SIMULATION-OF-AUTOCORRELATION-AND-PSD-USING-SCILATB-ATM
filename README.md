# EXP-NO.6-SIMULATION-OF-AUTOCORRELATION-AND-PSD-USING-SCILATB-ATM

# EQUIPMENTS Needed

•	Computer with i3 Processor
•	SCI LAB

# THEORY:
The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.

# Algorithm
1.	Load or Define the Signal: Input your time-domain signal.

2.	Compute Autocorrelation: Calculate the autocorrelation function of the signal.

3.	Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.

4.	Plot Results: Visualize the autocorrelation function and PSD.

# PROCEDURE

•	Refer Algorithms and write code for the experiment.

•	Open SCILAB in System

•	Type your code in New Editor

•	Save the file

•	Execute the code

•	If any Error, correct it in code and execute again

•	Verify the generated waveform using Tabulation and Model Waveform

# PROGRAM


clc

clear all;

t=0:0.01:2*3.14;

x=cos(12*t);

subplot(3,2,1); 

plot(x); 

au=xcorr(x,x);

subplot (3,2,2);

plot (au); 

v=fft(au); 

subplot(3,2,3);

plot(abs(v)); 

fw=fft(x); 

subplot(3,2,4)

plot(fw); 

fw2=(abs(fw)).^2;

subplot(3,2,5); 

plot(fw2);

# OUTPUT

<img width="768" height="710" alt="image" src="https://github.com/user-attachments/assets/d708d84c-624f-4e57-ac40-01274ce085bc" />

# RESULT
Thus the Autocorrelation and PSD are executed in Scilab and output is verified.





