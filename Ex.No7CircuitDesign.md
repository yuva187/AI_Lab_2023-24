# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE: 15/04/2025                                                                            
### REGISTER NUMBER : 212222060311
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

### Program:
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
### Output:
![Screenshot 2025-04-15 141728](https://github.com/user-attachments/assets/a671c51a-b69b-48d4-9bf0-1e927b498590)


### Result:
Thus the truth table of circuit verified sucessfully.
