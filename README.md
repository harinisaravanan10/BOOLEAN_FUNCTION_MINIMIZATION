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

Developed by:HARINI S RegisterNumber:212223040058

**RTL realization**

![image](https://github.com/harinisaravanan10/BOOLEAN_FUNCTION_MINIMIZATION/assets/149035598/2d092898-31f8-4a82-babf-eb644f3701cf)


**Truth table**

![image](https://github.com/harinisaravanan10/BOOLEAN_FUNCTION_MINIMIZATION/assets/149035598/fa5fb2d5-128a-46b9-a392-727d8baf65b9)


**Timing Diagram**

![image](https://github.com/harinisaravanan10/BOOLEAN_FUNCTION_MINIMIZATION/assets/149035598/4e93e10d-014b-4a96-87ef-846b5b57ce5f)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
