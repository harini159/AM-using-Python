
# AM using Python

EXP NO: 5 GENERATION AND DETECTION OF AM

AIM:

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries.

Apparatus Required:

1. Software: Python with NumPy and Matplotlib libraries 
2. Hardware: Personal Computer 

THEORY:

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of the message signal. The general form of an AM signal is:
                    s(t)=[Ac​+Am​cos(2πfm​t)]cos(2πfc​t)
                    where:
                    Ac is the amplitude of the carrier signal.
                    Am is the amplitude of the message signal.
                    fc is the frequency of the carrier signal.
                    fm is the frequency of the message signal.
                    t is time.

Note: Keep all the switch faults in off position.

Algorithm:

1.Set Up the Python Environment: Ensure that Python is installed on your system. You can use 
Anaconda for managing Python packages and environments, or any other Python IDE of your 
choice. 
2. Import Necessary Libraries: Import the math library in Python. 
3. Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling 
frequency. 
4. Generate Time Axis: Create a time vector for the signal duration. 
5. Generate Message Signal: Define the message signal as a cosine/sin wave. 
6. Generate Carrier Signal: Define the carrier signal as a cosine/sin wave. 
7. Modulate Signal: Apply the AM formula to obtain the modulated signal. 
8. Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.
 
Program:
```
 import numpy as np
   import matplotlib.pyplot as plt
   Am=2.19
   fm=284
   fs=28400
   Ac=3.19
   fc=2840
   t=np.arange(0,2/fm,1/fs)
   m=Am*np.cos(2*3.14*fm*t)
   plt.subplot(3,1,1)
   plt.plot(t,m)
   c=Ac*np.cos(2*3.14*fc*t)
   plt.subplot(3,1,2)
   plt.plot(t,c)
   Eam=(Ac+(Am*np.cos(2*3.14*fm*t)))*np.cos(2*3.14*fc*t)
   plt.subplot(3,1,3)
   plt.plot(t,Eam)
   plt.tight_layout()
   plt.show()
```
MODEL GRAPH:

<img width="691" height="538" alt="image" src="https://github.com/user-attachments/assets/7e275ca3-650b-4ccf-96dc-2c95fa3d0ff9" />

Output Waveform:

<img width="768" height="582" alt="Screenshot 2025-09-17 085949" src="https://github.com/user-attachments/assets/c065f8d0-956d-41ad-ac6f-d1d300eab6f9" />


TABULATION:

![am py](https://github.com/user-attachments/assets/0b0aebaa-5335-438d-966c-df2bb145eb01)


Calculation:
   1. ma (Theory) = am/ac = 0.68
   2. ma(Practical) = (Emax-Emin)/(Emax+Emin) = 10.4

RESULT:

Thus the amplitude modulation and demodulation is experimentally done and the output is verified.








