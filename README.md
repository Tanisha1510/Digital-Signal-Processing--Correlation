# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows

% INPUT SIGNAL-1
a=input('enter the starting x(n)');
x=input('Enter the x(n) sequence');
n=a:l:length(x)+a-l;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')

% INPUT SIGNAL 2
b=input('enter the starting y(n)');
y=input('Enter the y(n) sequence');
m=input('enter the ending y(n)');
n1=b:l:length(y)+b-l;

figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')

% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x);
n2=a-m:l:length(out1)+a-m-l;
figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title('Discrete auto correlated waveform')

% DISCRETE CROSS CORRELATED SIGNAL
Out2=xcorr(x,y);
n3=a-m:l:length(Out2)+a-m-l;
figure(4)
stem(n3,Out2)
xlabel('Time')
ylabel('Amplitude')
title('Discrete cross correlated waveform')
```
## OUTPUT:
<img width="505" height="453" alt="image" src="https://github.com/user-attachments/assets/8fd8ac8f-587d-4d76-a7bc-6a94ef9a12a9" />
<img width="497" height="445" alt="image" src="https://github.com/user-attachments/assets/a7e2db3c-1f95-4b8f-b689-742f429aa871" />
<img width="545" height="488" alt="image" src="https://github.com/user-attachments/assets/949f0f8e-0350-4da9-b4fa-f524f04ec3c2" />
<img width="548" height="491" alt="image" src="https://github.com/user-attachments/assets/1d3c8867-1bcf-4141-bb35-de0122eaa250" />


## RESULT:
<img width="965" height="248" alt="image" src="https://github.com/user-attachments/assets/d83fff55-a9fb-4a9c-9ead-b4b789335a9c" />

