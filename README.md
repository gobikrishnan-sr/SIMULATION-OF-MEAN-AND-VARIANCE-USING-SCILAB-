# SIMULATION-OF-MEAN-AND-VARIANCE-USING-SCILAB-
## AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output. 

## EQUIPMENTS NEEDED:

.Computer with i3 Processor 

.SCI LAB 

## ALGORITHM:

1. Define the Function: Specify the function you want to simulate. For example, 
f(x)=sin⁡(x)f(x)=sin(x) or any other function. 
2. Generate Sample Points: Decide on the range and the number of sample points. Generate 
these sample points within the desired range. 
3. Evaluate the Function: Compute the function values at each of these sample points. 
4. Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the 
mean and variance of the computed function values. 
5. Display Results: Output the computed mean variance and Cross Correlation 

## PROCEDURE:

1.Refer Algorithms and write code for the experiment. 

2.Open SCILAB in System 

3.Type your code in New Editor 

4.Save the file 

5.Execute the code If any Error, correct it in code and execute again 
  
6.Verify the generated results

## PROGRAM:
```
function X=f(x),
    z=6*(1+x)^2,
    X=x*z
endfunction
a=0;
b=1;
EX=intg(a,b,f)
function Y=c(y),
    z=6*(1+y)^2,
    Y=y*z
endfunction
EY=intg(a,b,c);
disp("Mean of X =",EX)
disp("Mean of Y =",EY)
function X=g(x),
    z=6*(1+x)^2,
    X=x^2*z
endfunction
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y)
    z=6*(1+y)^2,
    Y=y^2*z
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp("Variance of X",vX2);
disp("Variance of Y",vY2);
x=input("type in the reference sequence=");
y=input("type in the second sequence=");
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);
```

## OUTPUT GRAPH:
<img width="1913" height="1052" alt="image" src="https://github.com/user-attachments/assets/0e9d899b-c136-436c-82c6-c47adecfdd95" />


## Calculation:
![WhatsApp Image 2025-11-23 at 17 08 54_411367fd](https://github.com/user-attachments/assets/61e8aef9-aeee-45ad-92ef-449797b6f320)


## RESULT:
The simulation of mean and variance using Scilab successfully calculates the average value and the spread of the given data set. The results show that the mean represents the central tendency of the data, while the variance indicates how widely the values are distributed around the mean. The experiment confirms the accuracy of Scilab’s built-in functions in computing statistical parameters. Overall, the simulation clearly demonstrates the importance of mean and variance in analyzing numerical data.


