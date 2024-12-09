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
 a b sum (a ^ b) carry (a & b) 0 0 0 0 0 1 1 0 1 0 1 0 1 1 0 1

 ![Screenshot 2024-12-03 141838](https://github.com/user-attachments/assets/3793c770-6e20-4e48-bedc-14c5265f1446)

 a b difference (a ⊕ b) borrow (~a & b) 0 0 0 0 0 1 1 1 1 0 1 0 1 1 0 0 

 ![Screenshot 2024-12-03 141949](https://github.com/user-attachments/assets/a065f49d-6cba-44fa-97e5-fe718cb34d59)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

 module ha(a,b,sum,carry);
 input a,b;
 output sum,carry;
 assign sum= (a ^ b);
 assign carry= ( a & b);
 endmodule
 
 Half Subractor
 module hs(a,b,difference,borrow);
 input a,b;
 output difference,borrow;
 assign difference= (a ^ b);
 assign borrow= ( ~a & b);
 endmodule

Developed by: R.karthik padmanaban
RegisterNumber:24001743

**RTL Schematic**

![Screenshot 2024-12-09 192117](https://github.com/user-attachments/assets/909424c3-d529-47d4-8ecc-27624949a2f3)

![Screenshot 2024-12-09 192213](https://github.com/user-attachments/assets/7771b045-5e33-4db7-921c-91321e713f7f)


**Output/TIMING Waveform**

![Screenshot 2024-12-09 192323](https://github.com/user-attachments/assets/8c84f611-6fb6-4b07-968e-40f7e09954a0)

![Screenshot 2024-12-09 192415](https://github.com/user-attachments/assets/b395f2da-1cc3-442e-9d4b-a240d32666ad)


**Result:**
 Thus the given half adder and half subtractor fuctions are implemented and their operators are verified using Verilog programming

