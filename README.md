# Mataveid V4.0
Mataveid is a basic system identification toolbox for both GNU Octave and MATLAB®. Mataveid is based on the power of linear algebra and the library is easy to use. Subspace identification, realization theory and least square polynomial models are main focus in this project.

# Reports:

Mataveid contains subspace identification and realization identification algorithms. They can be quite hard to understand, compared to ARX, ARMAX, OE, TF models, so I highly recommend to read reports about the subspace identification and realization identification algorithm, to understand how the MATLAB/Octave functions code are written. The reports can be found in the folder "reports".

# Starting

Always start with help command of each function

```matlab
>> help era
'era' is a function from the file /home/hp/Dokument/Reglerteknik/mataveid/era.m

 Eigensystem Realization Algorithm
 Input: g(markov parameters), nu(number of inputs), sampleTime, delay(optional)
 Output: sysd(Discrete state space model)
 Example 1: [sysd] = era(g, nu, sampleTime, delay);
 Author: Daniel Mårtensson, November 2017

>>
```

# Typical use
# Ho-Kalman algorithm 
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/hokalman.png)
# Eigensystem Realization Algorithm
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/era.png)
# Eigensystem Realization Algorithm - Data Correlation
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/eradc.png)
# Step Based Realization
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/sbr.png)
# Observer/Kalman Filter Identification
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/okid.png)
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/okid2.png)
# Multivariable Subspace Identification
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/moesp.png)
# Past Input Multivariable Subspace Identification
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/pimoesp.png)
# Numerical Algorithms For Subspace State Space System IDentification
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/n4sid.png)
# Multivariable Numerical Algorithms For Subspace State Space System IDentification
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/MIMOn4sid.png)
# Arbitrary Subspace Algorithm  
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/asa.png)
# Orthogonal Decomposition
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/ort.png)
# Autoregressive Exogenous Model
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/arx.png)
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/arx2.png)
# Transfer function estimation
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/arxtf.png)
# Autoregressive–moving-average
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/armax.png)
# Spectral Analysis
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/spa.png)
# Smoothing
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/smoothing.png)
# Moving average
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/movingaverage.png)
# Linear Least Square best fit
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/leastsquare.png)
# Moving average 2
![alt text](https://github.com/DanielMartensson/mataveid/blob/master/pictures/moavg2.png)


# Install
To install Mataveid, download the folder "sourcecode" and place it where you want it. Then the following code need to be written in the terminal of your MATLAB® or GNU Octave program.

```matlab
path('path/to/the/sourcecode/folder/where/all/matave/files/are/mataveid', path)
savepath
```

Example:
```matlab
path('/home/hp/Dokument/Reglerteknik/mataveid', path)
savepath
```

Important! All the .m files need to be inside the folder mataveid if you want the update function to work.

# Update
Write this inside the terminal. Then Mataveid is going to download new .m files to mataveid from GitHub

```matlab
updatemataveid
```



# Requirements 
* Installation of Matavecontrol package https://github.com/DanielMartensson/matavecontrol

