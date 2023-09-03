NAME: SHALINI.K

REGISTER NO: 212222240095

# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit 

### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
### Theory:
Adders are digital circuits that carry out addition of numbers.

### Half Adder:
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder:
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 

![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

1.Connect the supply (+5V) to the circuit
2.Switch ON the main switch
3.If the output is 1, then the led glows.

### Program:
/*
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SHALINI.K
RegisterNumber:  212222240095
1. Program to design a half adder:
module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule
2. Program to design a full adder:
module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
```
*/

### TRUTH TABLE :

![image](https://github.com/shalinikannan23/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118656529/071d70fb-4c92-40e9-baaa-f56274f27c3e)

![image](https://github.com/shalinikannan23/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118656529/a396217f-e601-47ce-b321-17cefd322fb3)

## RTL REALIZATION:

HALF ADDER

![image](https://github.com/shalinikannan23/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118656529/a0497e4e-162c-402e-b971-93c0cdb831c4)

FULL ADDER

![image](https://github.com/shalinikannan23/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118656529/a577c9a0-1303-4ad5-ad50-66a9ad0c8c8c)

## OUTPUT WAVEFORM:

HALF ADDER

![image](https://github.com/shalinikannan23/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118656529/62140556-a298-4dec-bd48-d87caf45e797)

FULL ADDER

![image](https://github.com/shalinikannan23/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118656529/3cdce6fc-c5c4-4e8c-a1b7-1ca50a92ddc8)

### Result:

Thus the half adder and full adder circuit are designed and the truth table for half adder and full
adder are verified.
