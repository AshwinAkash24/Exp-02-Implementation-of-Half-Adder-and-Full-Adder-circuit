```
Name:M.Ashwin Akash
Reference number:23009906
```
# Exp-02-Implementation of Half Adder and Full Adder circuit

# AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

# Theory
Adders are digital circuits that carry out addition of numbers.

# Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

# Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

# Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

# Figure -02 FULL ADDER 

# Procedure
```
Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
```
# Program:
```
HALF ADDER:
module Halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a*b;
endmodule

FULLADDER:
module fulladder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry=a*b+b*c+c*a;
endmodule

```
# RTL realization:
![Screenshot 2023-11-28 105145](https://github.com/AshwinAkash24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979248/04fb1e16-e207-4a80-83e4-51664d70f902)
# ![Screenshot 2023-11-28 110310](https://github.com/AshwinAkash24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979248/c8a4e0e3-9f3a-4141-8343-4ab5f2161294)

# Truth Table:
![Screenshot 2023-11-28 105603](https://github.com/AshwinAkash24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979248/1ac5c40a-250d-4b9d-9e8a-3fe0bd41fff2)
# ![YUDUDY](https://github.com/AshwinAkash24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979248/bbebb59b-5347-4015-a8fc-c499cd4bc172)

# Timing Diagram:
![Screenshot 2023-11-28 103725](https://github.com/AshwinAkash24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979248/913997ec-a839-4b66-8811-06323b44fbb2)
![Screenshot 2023-11-28 110638](https://github.com/AshwinAkash24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979248/67139654-70f5-4937-ba32-3ad611d5c059)

# Result:
Hence, the implementation of half adder and full adder circuit is successful.
