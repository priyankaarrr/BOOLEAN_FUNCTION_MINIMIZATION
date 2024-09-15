# BOOLEAN_FUNCTION_MINIMIZATION

# Name: priyanka R
# Reg no: 212223220081

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:** 
Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime

**Theory**
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
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
**RTL realization**
![image](https://github.com/user-attachments/assets/e4dd0478-b2ed-4eeb-9e32-6b53834a0ea0)

**Truth Table**
![image](https://github.com/user-attachments/assets/c65ea62a-9f46-4eee-9efe-c429e171d0ab)


**Timing Diagram**
![image](https://github.com/user-attachments/assets/662f5121-4ea9-42f4-b500-aa660363995a)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

