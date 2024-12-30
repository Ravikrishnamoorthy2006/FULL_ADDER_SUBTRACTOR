# FULL_ADDER_SUBTRACTOR

Name : D.Ravikrishnamoorthy

Ref no : 212224040271

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

1. Type the program in quartus software.
2. Compile and run the program
3. Generate the RTL schematic and save the logic diagram
4. Create nodes for inputs and outputs to generate the timing diagram
5. For different input combinations genereate the timing diagram.

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

module fulladd(

input a,b.c,

output sum,carry);

wire w1,w2,w3;

assign sum=a^b^c;

assign w1=a&b;

assign w2=b&c;

assign carry = w1|w2|w3;

endmodule

module fullsub(a,b,c,diff,borr);

input a,b,c;

output diff,borr;

wire w1,w2,w3,w4,w5,w6;

xor g1(diff,a,b,c);

and g2(w4,w1,b);

and g3(w5,w1,b);

and g4(w6,b,c);

or g5(borr,w4,w5,w6);

endmodule

Developed by: D.Ravikrishnamoorthy

RegisterNumber: 212224040271

*/

**RTL Schematic**

![Screenshot 2024-12-30 190917](https://github.com/user-attachments/assets/4f8e1d8e-e7d2-40ea-b91d-a01e59a077f6)


![Screenshot 2024-12-30 190934](https://github.com/user-attachments/assets/4287163e-bd43-4a52-995d-6cba2d6657fe)



**Output Timing Waveform**

![Screenshot 2024-12-30 190954](https://github.com/user-attachments/assets/b7bafe2a-a882-4485-a7b3-86836b3425bb)


![Screenshot 2024-12-30 191026](https://github.com/user-attachments/assets/1a05561b-fbee-43d6-8335-441eb45ee81f)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



