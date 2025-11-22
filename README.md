# Mean-Variance-And-Cross-Correlation:

## Aim: 

To write a program for mean, variance and cross correlation in SCILAB and verify the output.

## EQUIPMENTS Needed:

• Computer with i3 Processor • SCI LAB

## Algorithm:

Define the Function:
Specify the function you want to simulate.
For example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.
Generate Sample Points:
Decide on the range and the number of sample points.
Generate these sample points within the desired range.
Evaluate the Function: Compute the function values at each of these sample points.
Compute Mean, Variance and Cross Correlation:
Use Scilab's functions to calculate the mean and variance of the computed function values.
Display Results:
Output the computed mean variance and Cross Correlation PROCEDURE 
• Refer Algorithms and write code for the experiment. 
• Open SCILAB in System • 
Type your code in New Editor:
• Save the file
• Execute the code 
• If any Error, correct it in code and execute again 
• Verify the generated results.

## Code:
```
function X=f(x)
    z=5 * (1-x)^2;
    X=x*z;
endfunction
a=2;
b=3;
EX=intg(a,b,f);
function Y=c(y)
    z=5 * (1-y)^2;
    Y=y*z;
endfunction
EY=intg(a,b,c);
disp(EX,"i)Mean of X=")
disp(EY,"Mean of Y=")

function X=g(x)
    z=3 * (1-x)^2;
    X=x **2 *z;
endfunction
a=2;
b=3;
EX2=intg(a,b,g);
function Y=h(y)
    z=3 * (1-y)^2;
    Y=y **2 *z;
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX) **2;
vY2=EY2-(EY) **2;
disp(vX2,"ii)Variance of X");
disp(vY2,"Variance of Y");

x=input("type in the reference sequence=");
y=input("type in the reference sequence=");
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);
```
## Output:

![WhatsApp Image 2025-11-20 at 17 57 00_ea6ae754](https://github.com/user-attachments/assets/8fc10509-f5ce-4244-b44c-322acf05067b)

## Calculation:

![WhatsApp Image 2025-11-22 at 20 12 21_1f98bbe1](https://github.com/user-attachments/assets/e6e8572b-d958-42f4-a155-9563daf73889)
![WhatsApp Image 2025-11-22 at 20 12 51_6c15b144](https://github.com/user-attachments/assets/19ce8011-7b28-48d7-ae2b-6dcda88054f5)
![WhatsApp Image 2025-11-22 at 20 13 11_2e15dc6a](https://github.com/user-attachments/assets/c4d0e3a8-c2d6-41fe-a389-c9ddcb75de10)




i) Mean of X = 112.95 ;Mean of Y = 112.97

ii) Variance of X =-12,271.7; Variance of Y =-12,291.6

Cross Correlation: Type in the reference sequence = [1 2 3 4 5 6 7 8]

Type in the second sequence = [2 1 3 5 6 3 5 9]

## Result:

Thus the mean , variance and cross correlation are executed in Scilab and output is verified
