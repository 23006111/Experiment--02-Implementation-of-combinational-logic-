# Experiment--02-Implementation-of-combinational-logic

Name:Ramya P
Ref No:23006111
 
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
module exp_2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
## RTL realization
![image](https://github.com/23006111/Experiment--02-Implementation-of-combinational-logic-/assets/145981696/88d33729-d6c0-4797-a84d-601e5912ebe7)
![image](https://github.com/23006111/Experiment--02-Implementation-of-combinational-logic-/assets/145981696/5ef5c40d-9d07-47fd-9447-3b58c45553cd)




## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
