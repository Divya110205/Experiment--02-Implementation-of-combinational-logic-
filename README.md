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
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.


## Procedure
Step 1: 

Create a project with required entities.

Step 2:

Create a module along with respective file name.

Step 3:

Run the respective programs for the given equations.

Step 4:

Run the module and get the respective RTL outputs.

Step 5:

Create university program(VWF) for getting timing diagram.

Step 6:

Give the respective inputs for timing diagram and obtain the results.
## Program:
F1:

module ff(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1 = (~b&~d) | (~a&b&d) | (a&b&~c);

endmodule

F2:

module de (w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2 = (x&y)|(w&y)|(~y&z);

endmodule
Developed by: A.DIVYA
RegisterNumber: 212222230034 
*/
## RTL realization
## F1
![f1 rtl](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/029331d5-e82d-4b3e-9c0a-58de6af1fb76)

## F2
![f2 rtl](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/d618a026-b3bc-4445-ae04-9e1e55f13bbc)

## Output:

## Timing Diagram
## F1
![f1 td](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/dfc3ae1f-ab5a-4dd5-a447-fa5fd1b2267e)

## F2 
![f2 td](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/8938c25f-0a89-431d-9c47-ee1053e17ea1)

## Truth Table
![tt](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/2992336b-e9b1-4be4-b11c-2fe9db388021)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
