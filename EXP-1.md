# GENERATION OF STANDARD DISCRETE-TIME SIGNALS
# AIM:
To generate and plot standard discrete-time signals using MATLAB.
# APPARATUS REQUIRED:
•	Computer / Laptop
•	MATLAB software
# THEORY:
Discrete-time signals are signals defined only at integer values of time (n).
These signals are basic building blocks in Digital Signal Processing (DSP) and are used for system analysis, filtering, and signal modeling.
Standard discrete-time signals include:
	Unit Impulse
	Unit Step
	Ramp
	Exponential
	Sinusoidal
	Damped Sinusoidal
In MATLAB, discrete-time signals are represented using vectors and plotted using the stem() command.
 Standard Discrete-Time Signals
 
🔹 1. Unit Impulse Signal
δ(n)={1,n=0
	  0,n≠0}

🔹 2. Unit Step Signal
u(n)={1,n≥0
      0,&n<0}

🔹 3. Ramp Signal
r(n)=n⋅u(n)

🔹 4. Exponential Signal
x(n)=a^n

🔹 5. Sinusoidal Signal
x(n)=sin⁡(ωn)

🔹 6. Damped Sinusoidal Signal
x(n)=a^n sin⁡(ωn)

# ALGORITHM:
1.	Start the program
2.	Define the sample index n
3.	Generate each standard discrete-time signal
4.	Plot the signal using stem()
5.	Label the axes and title
6.	Stop the program

# MATLAB CODE:
```
% GENERATION OF STANDARD DISCRETE-TIME SIGNALS

clc;
clear;
close all;

%% Sample index
n = -10:10;

%% 1. Unit Impulse Signal
x1 = (n == 0);
figure;
stem(n, x1, 'filled');
title('Unit Impulse Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 2. Unit Step Signal
x2 = (n >= 0);
figure;
stem(n, x2, 'filled');
title('Unit Step Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 3. Ramp Signal
n1 = 0:10;
x3 = n1;
figure;
stem(n1, x3, 'filled');
title('Ramp Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 4. Exponential Signal
a = 0.8;
x4 = a.^n1;
figure;
stem(n1, x4, 'filled');
title('Exponential Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 5. Sinusoidal Signal
x5 = sin(0.3*pi*n1);
figure;
stem(n1, x5, 'filled');
title('Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 6. Damped Sinusoidal Signal
x6 = (0.9.^n1).*sin(0.4*pi*n1);
figure;
stem(n1, x6, 'filled');
title('Damped Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;
```

# OUTPUT GRAPH:
1. Unit Impulse Signal
<img width="1230" height="817" alt="image" src="https://github.com/user-attachments/assets/1cdd8dba-214a-4e28-8fdd-e6f5458e019e" />
2. Unit Step Signal
<img width="1230" height="817" alt="image" src="https://github.com/user-attachments/assets/a6ff5d3f-325d-490a-9bf2-579cbccb5846" />
3. Ramp Signal
<img width="1225" height="817" alt="image" src="https://github.com/user-attachments/assets/dfab6c8d-cb5f-4fa3-a281-2c0d0a98a54b" />
4. Exponential Signal
<img width="1230" height="817" alt="image" src="https://github.com/user-attachments/assets/d596f5f7-e035-4304-a0e2-978142259d79" />
5. Sinusoidal Signal
<img width="1237" height="817" alt="image" src="https://github.com/user-attachments/assets/8c480dd7-31dd-4499-9849-e3ba086c5b30" />
6. Damped Sinusoidal Signal
<img width="1237" height="817" alt="image" src="https://github.com/user-attachments/assets/cad0f26a-cfb7-42c3-952b-537e434052a6" />


# Result :
Thus, standard discrete-time signals were successfully generated and plotted using MATLAB.



