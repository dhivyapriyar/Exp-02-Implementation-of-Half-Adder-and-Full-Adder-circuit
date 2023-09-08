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

Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows

### Program
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Dhivyapriya.R

RegisterNumber:212222230032  

## half adder

module exp3 (a,b,sum,carry);

input a,b;

output sum,carry;

assign sum = (a^b);

assign carry = (a&b);

endmodule

## Full adder

module exp3f (a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum = (a^b^c);

assign carry = ((a&b)|(a^b)&c);

endmodul

```
### Output:
### RTL

Halfadder

![exp3 1](https://github.com/dhivyapriyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477552/d0645b84-c930-424c-b4c5-215f91e8d1ff)

Fulladder

![exp3 2](https://github.com/dhivyapriyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477552/4aecc9e4-78f5-4cfb-8536-52e10e7573b6)

### TIMING DIAGRAM

Halfadder

![exp3 4](https://github.com/dhivyapriyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477552/de2e3227-7167-4911-8f8b-b081f7923c84)

Fulladder

![exp3 5](https://github.com/dhivyapriyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477552/e42bcee0-85d4-41c7-a727-4f2d8e239ab5)

### TRUTH TABLE 

Halfadder

![exp3 6](https://github.com/dhivyapriyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477552/1baac84a-7667-410d-9751-8a8fd6e88c20)

Fulladder

![exp3 7](https://github.com/dhivyapriyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477552/d341c730-3768-4def-a674-b7415610647e)

### Result:

Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
