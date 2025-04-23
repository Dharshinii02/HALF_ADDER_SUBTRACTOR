# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
![Screenshot 2025-04-23 143802](https://github.com/user-attachments/assets/1a4ff5e4-439b-4f8c-a456-12bc84ddd0a3)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
i)HALF ADDER

  module HF(a,b,sum,carry); 
  input a,b;
  output sum,carry;
  assign sum= (a ^ b);
  assign carry= ( a & b);
  endmodule


ii)HALF SUBTRACTOR

 module HF(a,b,difference,borrow);
 input a,b;
 output difference,borrow;
 assign difference= (a ^ b);
 assign borrow= ( ~a & b);
 endmodule
```

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:Dharshini J RegisterNumber:*/ 212224240036

**RTL Schematic**
![Screenshot 2025-04-23 143607](https://github.com/user-attachments/assets/345cc6c9-edd1-442c-a24c-c3629470096f)
![Screenshot 2025-04-23 143617](https://github.com/user-attachments/assets/91f6d4f1-9d72-4020-a682-d3b32ba5e9f3)


**Output/TIMING Waveform**
![Screenshot 2025-04-23 143634](https://github.com/user-attachments/assets/993448cc-46ab-4894-8711-5db498bb4bb2)
![Screenshot 2025-04-23 143647](https://github.com/user-attachments/assets/7c36b323-5b35-4a8e-8963-9ebdb74f90a4)


**Result:**
Thus the Half-adder and Half-subtractor are studied and truth table and logic gates are verified successfully.
