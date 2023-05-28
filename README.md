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

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: M.Saidharshan
RegisterNumber: 212222050049

### Program:
```
module halfadder(a,b,sum,carry);
input a,b;
output sum carry;
xor (sum,a,b,);
and(carry,a,b);
endmodule

full adder
program:
module Fulladder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=((a^b)^c;
assign carry-=((a&b)|(b&c)|(c&a));
endmodule
```

Logic symbol & Truthtable
![241402414-2647b3da-5bc0-497e-b0f7-8f4d53492db0](https://github.com/maaplasai7/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/134155273/8f8ab531-a9cb-4e8e-ba74-f3db0c4499f8)

RTL realization
![241402445-b641c909-45aa-4c9d-bcca-a5c4d50f56be](https://github.com/maaplasai7/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/134155273/1cb9dfb8-ba1d-42bd-80b8-79618b118b35)


### Output:
### RTL
![b98fcf3d-c47f-4f1a-b1cc-d472d3192a34](https://github.com/maaplasai7/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/134155273/55b3214a-80fd-4baa-852e-d5bdd3fc8a4e)



### TIMING DIAGRAM
![8f16a9d7-dcc6-4d56-9603-7c994293d8b1](https://github.com/maaplasai7/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/134155273/fe99326a-b07b-4f00-95a3-7bbfeca50b29)



### TRUTH TABLE 

### Result:
The  experiment half and full adder experiment is submitted
