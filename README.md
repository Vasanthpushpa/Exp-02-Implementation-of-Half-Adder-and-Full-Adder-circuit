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
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:VASANTH P 
RegisterNumber:212222240113
module VASANTH(x,y,s,c);
input x,y;
output s,c;
xor(s,x,y);
and(c,x,y);
endmodule

module full_adder(x, y, z, s, c, x1, x2, x3);
input x,  y,z;
output s ,c, x1, x2, x3;
xor(x1, x, y);
xor(s, x1, z);
and(x2, x, y);
and(x3, x1, z);
or(c, x2, x3);
endmodule
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
![image](https://user-images.githubusercontent.com/119291100/234770371-b2e88aaf-36b0-4590-a551-93cf683b074a.png)
![image](https://user-images.githubusercontent.com/119291100/234770409-9752413a-59d0-49a5-8156-0dff74e639c1.png)

### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/119291100/234770445-2ac5b28c-ff1f-476f-9c68-b50ec5a85586.png)
![image](https://user-images.githubusercontent.com/119291100/234770476-02e9e48a-cbb7-4f1b-adda-b93fa6d4bb3b.png)


### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/119291100/234770506-baaaef34-4229-44fd-bc37-deb3b0f64104.png)
![image](https://user-images.githubusercontent.com/119291100/234770534-c7bdde7f-0404-4108-b1f4-a88160c90a74.png)


### Result:
Therefore,half adder and full adder is verified.
