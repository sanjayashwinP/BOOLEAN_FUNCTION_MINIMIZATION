# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
module combinationalcircuit(A,B,C,D,F1);
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
#### Developed By: Sanjay Ashwin P
#### Register No: 212224020181

**RTL realization**

![285831617-8766d4a1-0593-4b06-a5f4-8c977e44b4ad](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/f0108d3e-78c4-49fa-9661-c9d5bbf2b99b)

**Truth Table**

![285832032-236326de-e839-4fad-908b-bb236e0a13dd](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/399f99d5-79cc-443a-b54a-41d7a0326a5c)


**Timing Diagram**

![285832328-c7532fe5-12ef-476d-a070-ab42a2ea7636](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/3aa93f44-b173-448e-829e-90ac3afb0776)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

