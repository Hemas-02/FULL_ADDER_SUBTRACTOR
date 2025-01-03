

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

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by:24901252
RegisterNumber:Hemalatha.R
*/
ex04(sum,cout,a,b,cin)

output sum;

output cout;

input a;

input b;

input cin;

wire sl,cl,c2;

and(c2,sl,cin0

and(c2,sl,cin)

or(cout,c2,cl)

endmodule

full subractor module ex04a(df,bo,a,b,bin);

output df;

output bo;

input a;

input b;

input bin;

wire w1,w2,w3;

assign w1=a^b;

assign w2=(~a&b);

assign w3=(-w1&bin);

assign df-w1^bin;

assign bo-w2/w3;

end module

**RTL Schematic**
![Screenshot (96)](https://github.com/user-attachments/assets/9c32cd6e-37df-4d95-a705-891105a2b4a9)
![Screenshot (97)](https://github.com/user-attachments/assets/b6ab9aea-3515-4e19-b022-3e7df9cc3203)

**Output Timing Waveform**
![Screenshot (98)](https://github.com/user-attachments/assets/81d7899c-9f16-408c-898e-d251dae4f21f)
![Screenshot (99)](https://github.com/user-attachments/assets/59eb0278-e8d2-424a-a6c8-d2216a7ea9a8)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



