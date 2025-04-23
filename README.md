# HALF_ADDER_SUBTRACTOR
```
Developed by: Preethi.K
Register no.: 212224240118
```
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

![Screenshot 2025-04-23 160009](https://github.com/user-attachments/assets/8df5ac31-6106-4cb4-8b42-4b3acb775fda)
![Screenshot 2025-04-23 160024](https://github.com/user-attachments/assets/0868e24e-eb21-4b48-ad0c-ed618c9d848c)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
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
 assign borrow= ( ~a & b);
 endmodule
```

**RTL Schematic**

![Screenshot 2025-04-23 160049](https://github.com/user-attachments/assets/c3dd2650-f3a3-46c4-816b-0dbd0d7035c2)
![Screenshot 2025-04-23 160113](https://github.com/user-attachments/assets/4425f712-8627-490b-954f-cb6a65a57315)

**Output/TIMING Waveform**

![Screenshot 2025-04-23 160128](https://github.com/user-attachments/assets/169712b9-24de-4c37-bc5e-51ddb126923c)
![Screenshot 2025-04-23 160142](https://github.com/user-attachments/assets/d44ef0b6-0f1b-4e52-8a6c-752cc6e17773)

**Result:**
Thus the Half -adder and Half subtractor are studied and truth table and logic gates are verified successfully.
