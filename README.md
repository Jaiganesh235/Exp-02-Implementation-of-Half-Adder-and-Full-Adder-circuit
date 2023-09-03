```
NAME: S.JAIGANESH
REGISTER NO: 212222240037
```
# EXP-03-IMPLEMENTATION OF HALF ADDER AND FULL ADDER CIRCUIT


## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.


## EQUIPMENTS REQUIRED:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime


## THEORY:
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B 
    Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 
Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

### Figure -02 FULL ADDER 


## PROCEDURE:
1. Connect the supply (+5V) to the circuit
2. Switch ON the main switch
3. If the output is 1, then the led glows.


## PROGRAM:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: S.Jaiganesh
RegisterNumber: 212222240037

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

## TRUTH TABLE:
### HALF ADDER
![image](https://github.com/Jaiganesh235/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118657189/19858532-c597-436f-9664-fe5791928f78)
 
### FULL ADDER
![image](https://github.com/Jaiganesh235/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118657189/afc4522a-f291-40a5-845c-32c14bb92999)




## RTL REALIZATION:
### HALF ADDER
![image](https://github.com/Jaiganesh235/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118657189/f7cfff41-9671-4c3c-b523-7edd2074233b)

### FULL ADDER
![image](https://github.com/Jaiganesh235/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118657189/7cb66c1f-4a79-4103-99ca-b50942d250cd)


## OUTPUT WAVEFORM:
### HALF ADDER
![image](https://github.com/Jaiganesh235/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118657189/c3ece2e7-b7ce-4c6f-961a-ebebbec90493)
 
### FULL ADDER
![image](https://github.com/Jaiganesh235/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118657189/dfd139bf-43ed-4300-80e0-398ca22f45ff)


## RESULT:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
