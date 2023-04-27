# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
```
module combination(a,b,c,d,x,y,z,w,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire a1,a2,a3,a4,a5,b1,b2,b3,b4,b5;
assign a1=((~a)&(~b)&(~c)&(~d));
assign a2=((a)&(~c)&(~d));
assign a3=((~b)&(c)&(~d));
assign a4=((~a)&(b)&(c)&(d));
assign a5=((b)&(~c)&(d));
assign b1=((x)&(~y)&(z));
assign b2=((~x)&(~y)&(z));
assign b3=((~w)&(x)&(y));
assign b4=((w)&(~x)&(y));
assign b5=((w)&(x)&(y));
assign f1=(a1|a2|a3|a4|a5);
assign f2=(b1|b2|b3|b4|b5);
endmodule
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: BASKARAN.V
RegisterNumber:  212222230020
*/
## RTL realization

## Output:

## RTL
![dig1](https://user-images.githubusercontent.com/118703522/234770411-709d21ec-21ef-4cd7-af02-9138b4fdf8d1.png)
![dig2](https://user-images.githubusercontent.com/118703522/234770459-d9e72082-62c4-4cc2-8601-f054701a47ad.png)

## Timing Diagram:
![dig](https://user-images.githubusercontent.com/118703522/234770525-efc81621-b3a8-4ac6-a383-4c53d280f670.png)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
