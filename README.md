# Ex.No: 7 Logic Programming – Logic Circuit Design
## DATE: 15/04/2025
## REGISTER NUMBER :  212222060311
## AIM:
To write a logic program to design a circuit like half adder and half subtractor.

## Algorithm:
Start the Program
Design a AND gate logic if both inputs are 1 then output is 1.
Design a OR gate logic if any one of input is 1 then output is 1.
Design a XOR gate logic if both inputs are different then output is 1.
Design a NOT gate logic if input is 0 then output is 1.
Design a half adder and half subtractor using the rules.
Test the logic.
Stop the program.
## Program:
```
ha(A,B,Sum,Carry):-
    xor(A,B,Sum),
    and(A,B,Carry).
hs(A,B,Diff,Borrow):-
    xor(A,B,Diff),
    not(A,A_not),
    and(A_not,B,Borrow).
fa(A,B,Cin,S,Cout):-
    xor(A,B,X),
    xor(X,Cin,S),
    and(X,Cin,Y),
    and(A,B,Z),
    or(Y,Z,Cout).
and(0,0,0).
and(0,1,0).
and(1,1,1).
and(1,0,0).
xor(0,0,0).
xor(0,1,1).
xor(1,0,1).
xor(1,1,0).
not(0,1).
not(1,0).
or(0,1,1).
or(1,0,1).
or(0,0,0).
or(1,1,1).
```
## Output:
![image](https://github.com/user-attachments/assets/1353a1c7-dd88-4bf7-9da9-6da4df47dafe)

## Result:
Thus the truth table of circuit verified sucessfully.
