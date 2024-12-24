# BOOLEAN_FUNCTION_MINIMIZATION

Developed by: SANTHOSH SUDHAKAR

RegisterNumber: 24005023
```

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

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

## Logic symbol & Truthtable:
![image](https://github.com/user-attachments/assets/1d7095c0-4b7a-4fc8-ae44-7d86d9af7df3)
![image](https://github.com/user-attachments/assets/9a2c62bc-d0c9-41c0-8464-a55f9fbfb6fd)

**RTL realization**
![image](https://github.com/user-attachments/assets/9bd7785a-00ae-4eca-bfcf-794434576fed)

**Output:**
![image](https://github.com/user-attachments/assets/ed1d5001-582e-45c4-8096-0a5b0a7984af)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

