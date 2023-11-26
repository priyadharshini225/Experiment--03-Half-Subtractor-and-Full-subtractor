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

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: PRIYADHARSHINI S
RegisterNumber:  23003522
1. Program to design a half subtractor:

![hs code](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/9e0ad7d5-f0dd-4e7e-a098-dc233e95f1be)

3. Program to design a full subtractor:

![fs code](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/c8dae322-2d37-4376-982a-c09fb1ecaa2c)


## Output:

## Truthtable:
## HALF SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/c3f5f5da-4bc4-47d0-baf2-90381b3bdd14)
## FULL SUBTRACTOR:
![image](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/04cf3e64-7b10-435e-90b8-7dbcb78477bf)

##  RTL realization
## HALF SUBTRACTOR:
![hs](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/bd04dcf8-56b9-4bc5-a45b-5421c5ddd180)

## FULL SUBTRACTOR:
![fs](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/adff5403-0af1-4af3-bd46-0480a3dbe198)


## Timing diagram:
## HALF SUBTRACTOR:
![hs wave](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/a0be7c0e-2ab5-4d00-9e37-2558a24644d9)

## FULL SUBTRACTOR:
![fs wave](https://github.com/priyadharshini225/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/138849213/54b3110b-b244-4b83-a2b6-14cdce511295)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
