# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

 A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

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

![image](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/f4e0dc5c-6df7-46b1-90a8-fbdbcf6bb658)

**Truth Table**

![285832032-236326de-e839-4fad-908b-bb236e0a13dd](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/399f99d5-79cc-443a-b54a-41d7a0326a5c)

![image](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/86318cdd-6571-45dd-8e95-6458eb6074cc)

**Timing Diagram**

![image](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/07b5e0bd-6050-4fb7-86af-4113419d5e6e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

