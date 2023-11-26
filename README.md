# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure:
*Connect the supply (+5V) to the circuit. *Switch ON the main switch. *If the output is 1, then the led glows.

## Program:
```
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: PRIYADHARSHINI S
RegisterNumber:  23003522
1. Program to design a half subtractor:
module ex4(a,b,diff,borr);
input a,b;
output diff,borr;
assign diff=(a^b);
assign borr=((~a)&b);
endmodule 
2. Program to design a full subtractor:
module ex41(a,b,bin,diff,borr);
input a,b,bin;
output diff,borr;
assign diff=a^b^bin;
assign borr=((~a)&b)|(b&bin)|((~a)&bin);
endmodule
```

## Output:

## Truthtable:
## HALF SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/c3f5f5da-4bc4-47d0-baf2-90381b3bdd14)
## FULL SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/04cf3e64-7b10-435e-90b8-7dbcb78477bf)

##  RTL realization
## HALF SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/a9102d9c-8f3d-42ee-b833-55119c4b3760)
## FULL SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/c1b65584-4b0e-4240-b3c3-879d715d4bff)

## Timing diagram:
## HALF SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/e8d6aaee-4dea-4b34-a560-4806129e1ba8)
## FULL SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/ec0f84f3-6edd-4bd3-afa1-b696ac5085ca)


## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
