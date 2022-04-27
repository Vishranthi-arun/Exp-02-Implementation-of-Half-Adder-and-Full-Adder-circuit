# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 

![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

1. Connect the supply (+5V) to the circuit
2. Switch ON the main switch
3. If the output is 1, then the led glows.
### 
Program:
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Vishranthi A
RegisterNumber:  212221230124
HALF ADDER

module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule 

FULL ADDER

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
*/
```
### Output:
### half adder:
## Logic symbol:
![halfgate](https://user-images.githubusercontent.com/93427278/165533334-e000082f-b505-48cf-87c6-de8da89432ac.png)
## RTL Realization:
![hrtl](https://user-images.githubusercontent.com/93427278/165533571-574a651a-82b7-44d6-9908-21b4e0866772.png)
## Truth table:
![haddtable](https://user-images.githubusercontent.com/93427278/165533706-7fd73b06-99f5-4c8b-aae4-652837647db8.png)
## Timing Diagram:
![htiming](https://user-images.githubusercontent.com/93427278/165533752-b256ce09-6ae1-4898-996b-14d88bbcce35.png)

### FULL ADDER:
## Logic Symbol:
![fullgate](https://user-images.githubusercontent.com/93427278/165533886-afecbec3-57ec-448a-89c6-973b03ff38b1.png)
## RTL Realization:
![frtl](https://user-images.githubusercontent.com/93427278/165533967-006efb56-f048-4516-9c2a-b6b2f54d7ce2.png)
## Truth Table:
![faddtable](https://user-images.githubusercontent.com/93427278/165534055-e17f1728-6de9-4886-aac8-9ebf640e4810.png)
## Timing Diagram:
![ftiming](https://user-images.githubusercontent.com/93427278/165534121-a7f3e1ec-076e-449f-b77b-9edb38ab334f.png)

### Result:
 Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
