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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: PARVESHWARAN R 
RegisterNumber: 212225040295


**RTL realization**
```
module de2 (
    input A, B, C, D,
    output F
);

assign F = (~A & ~B & ~C & ~D) |
           ( A & ~C & ~D )     |
           (~B &  C & ~D )     |
           (~A &  B &  C &  D) |
           ( B & ~C &  D );

endmodule
```

**Output:**



**RTL**
<img width="662" height="375" alt="image" src="https://github.com/user-attachments/assets/ab1b46c4-db3e-445f-a219-52dfed3980f0" />



**Timing Diagram**
<img width="1536" height="357" alt="image" src="https://github.com/user-attachments/assets/ba199b02-4d38-40e1-962e-353688a00a44" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

