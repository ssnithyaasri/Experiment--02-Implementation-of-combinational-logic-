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
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.Combinational logic gates are digital circuits that produce outputs based solely on the current inputs. These gates are the building blocks for implementing digital systems and are used in a wide range of applications, including arithmetic and logic operations, memory devices, and control circuits.The two functions, F1 and F2, can be implemented using a combination of logic gates such as AND gates, OR gates, and NOT gates.
 

## Procedure

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.


## Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: NITHYAA SRI S S 

RegisterNumber: 212222230100 

```
module EX2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1= (~A)&(~B)&(~C)&(~D);
assign x2= (A)&(~C)&(~D);
assign x3= (~B)&(C)&(~D);
assign x4= (~A)&(B)&(C)&(D);
assign x5= (B)&(~C)&(D);
assign F1= x1|x2|x3|x4|x5;
endmodule 
```
## RTL realization

## Output:

## RTL DIAGRAM
## RTL realization
![output](Screenshot%202023-08-26%20211232.png)
## TRUTHTABLE
![output](Screenshot%202023-08-26%20095832.png)
## Timing Diagram
![output](Screenshot%202023-08-26%20211341.png)
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
