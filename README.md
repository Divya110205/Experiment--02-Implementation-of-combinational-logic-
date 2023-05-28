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
Step 1: Create a project with required entities.

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
##F1
![Screenshot (55)](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/f70c350d-4c5f-41e6-b721-3f47ec006a72)

##F2
![Screenshot (54)](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/aa6be979-4924-414a-a346-cad4a5dd432d)

## Output:

## Timing Diagram
##F1
![f1](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/333c0125-6369-47db-bd59-647e485dfa82)

##F2 
![f2](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/ef80b7d8-e5d5-4b72-998f-1c62bba2d807)

##Truth Table
![tt](https://github.com/Divya110205/Experiment--02-Implementation-of-combinational-logic-/assets/119404855/2992336b-e9b1-4be4-b11c-2fe9db388021)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
