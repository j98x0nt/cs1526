java c
ELEC ENG 2104 Digital Signal Processing
Assignment 3 – Filter Design  Spectral Analysis
Semester 2, 2024
InstructionsAttempt all questions.  Include Matlab plots in your submission.  Upload a single pdf file on MyUni.  No other formats will be accepted.  The total  mark for this assignment is 20.  Part  marks for each question are  listed. Presentation will be taken into account in the marking.This  is  an  individual  assignment.   Discussing  with  others  are encouraged  but  make  sure you only  submit work  that  is  entirely  your  own.    Including  code  templates  and  examples  from  MyUni  is  permitted  but make sure these are appropriately referenced.  Refer to the  University’s Academic  Integrity policy for details:
https://www.adelaide.edu.au/policies/230/
To complete this assignment, you need the file DSP2024_assigment3 .mat from MyUni.  Put  it in the same folder as your Matlab work files.Question 1. A continuous time signal xa (t) has a spectrum (Fourier transform) shown in figure 1. This signal is to be sampled into a discrete time signal x[n].  Suggest an appropriate sampling rate for this situation.  Briefly justify your answer.Figure 1: Spectrum of continuous time signal to be sampled.
The DT signal is quantised using an ADC with a resolution of 12 bits.  Estimate the signal to distortion ratio (SDR) of this quantisation scheme, stating any assumptions. [2 marks]
Question 2. A digital lowpass filter is needed to meet the following specifications:
• Passband edge ωp  = 0.24π
•  Stopband edge ωs  = 0.3π
• Passband ripple δp  = 0.2dB
• Stopband attenuation δs  = 30dB
(a)  Use the Matlab function fir1 to obtain a linear phase FIR windows-based design. [1 mark]
(b)  Use the Matlab function firls to obtain a linear phase FIR least square error design. [1 mark]
(c)  Use the  Matlab function firpm to obtain a linear phase FIR Parks-McClellan (equiripple) design. [1 mark]
(d)  Use the Matlab function ellip to obtain an elliptical IIR design. [1 mark]
(e)  Briefly compare the orders of the designs and hence comment on their implementation costs. [1 mark]
For parts (a)–(d), show the impulse response, magnitude response and group delay plots to demonstrate your design meets the specifications.  Clearly state any design parameters you have chosen.
Question  3. The  complex-valued  signal stor代 写ELEC ENG 2104 Digital Signal Processing Assignment 3 – Filter Design & Spectral Analysis Semester 2, 2024Matlab
代做程序编程语言ed  in  the  Matlab  variable  x3 consists of  mulitple sinusoidal components and corrupted by white noise.
(a)  Compute the DFT of the signal and plot the power spectral density (dB scale) as a function of frequency. From your spectrum, identify the frequency components which are present in the signal.  The relevant Matlab command is fft. [2 marks]
(b)  Now  compute a windowed  DFT of the signal  using  a  Hamming window and  plot the  resultant energy density spectrum.  Explain what you observe.  Use the Matlab command window to generate the Hamming window. [2 marks]
Question 4. Sketch the signal flow graphs for the
(a)  canonical implementation of the FIR filter with impulse response
h[n] ={1, −2,   5, −2,    1 }[1 mark]
(b)  first order parallel architecture of the IIR filter with transfer function
[1 mark]
(c)  cascade implementation of the  IIR filter with second order systems
[1 mark]
Question 5. (a)  Calculate and write the magnitude (|X[k]|) and phase (7X[k]) of the 8-point DFT of
x[n] ={1,   2,   3,    1,   2,   3,    1,   2 } .[1 mark]
(b)  Consider the two DT signals
x1 [n] ={1, −2, −4, −1,   3,   2 } ,
x2 [n] ={−1,   5,   3,   2, −2, −3} .
Calculate the circular convolutions x1 [n] ⊛ x2 [n] of these two signals for (i) N = 6, (ii) N = 10 and (iii) N = 12. Compare these outputs with the linear convolution x1 [n] * x2 [n]. [2 marks]
(c)  Use DFTs to calculate the output y[n] of the DT LSI system with impulse response h[n] and input x[n]
h[n] ={1, −1,   3, −1,    1 } ,
x[n] ={5, −8,    3, −1,   3,   6, −3,   8, −5,   0,   2,   5 } .You can use convolution to check the answer, but it will not attract any marks. [1 mark]
Question 6. Consider the causal DT LSI system,
y[n] + 1.27y[n − 1] + 0.81y[n − 2] = x[n].
The system’s input x[n] is a Gaussian white noise process with variance 1.
(a) What is the autocorrelation of the output process RY Y [l] and power spectral density SYY (ω)? [1 mark]
(b)  Simulate M  = 500 realisations of white noise inputs, using N = 128 samples per realisation.  Use the filter command to produce each output realisation and calculate its periodogram, i.e. squared magni- tude of its DFT. Average periodograms from all M realisations and compare the theoretical expectation from part (b). [1 mark]Total:  20 marks



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
