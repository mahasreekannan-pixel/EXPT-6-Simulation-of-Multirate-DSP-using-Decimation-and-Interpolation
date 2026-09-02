# EXPT-6-Simulation-of-Multirate-DSP-using-Decimation-and-Interpolation

# AIM: 

# To perform and verify Multirate-DSP-using-Decimation-and-Interpolation.

# APPARATUS REQUIRED: 
PC installed with SCILAB. 

# PROGRAM: 
<br>clear; 
<br>clc; 
<br>close; 
<br>n = 0:%pi/50:2*%pi; 
<br>x = sin(%pi*n); //original signal 
<br>M=input('Enter the downsampling factor'); 
<br>L=input('Enter the upsampling factor'); 
<br>//Down Sampling 
<br>downsampling_x = x(1:M:length(x)); 
<br>disp(x,'Input signal x(n)='); 
<br>disp(downsampling_x,'Downsampled Signal'); 
<br>figure(1); 
<br>subplot(2,1,1) 
<br>plot2d3(1:length(x),x); 
<br>xtitle('original singal') 
<br>subplot(2,1,2) 
<br>plot2d3(1:length(downsampling_x),downsampling_x); 
<br>xtitle('Downsampled Signal by a factor of M'); 
<br>//Upsampling 
<br>upsampling_x=[]; 
<br>for i=1:length(x) 
<br>upsampling_x(1,L*i)=x(i); 
<br>end 
<br>disp(x,'Input signal x(n)='); 
<br>disp(upsampling_x,'Upsampled Signal'); 
<br>figure(2); 
<br>subplot(2,1,1); 
<br>plot2d3(x); 
<br>title('original signal'); 
<br>subplot(2,1,2); 
<br>plot2d3(upsampling_x); 
<br>title('Upsampled Signal by a factor of L');


# OUTPUT: 
<img width="526" height="116" alt="image" src="https://github.com/user-attachments/assets/53862821-796f-4819-afe4-d780b057849e" />
<img width="455" height="377" alt="image" src="https://github.com/user-attachments/assets/dce93992-3dc4-4f55-b7e0-d42c9861efd5" />
<img width="455" height="373" alt="image" src="https://github.com/user-attachments/assets/ef137601-ebd7-4cf9-a80d-4264424defab" />


# RESULT: 
Thus the Multirate-DSP-using-Decimation-and-Interpolation using python was performed and verified.
