# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE:  15/04/2025                                                                         
### REGISTER NUMBER :  212222060311
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
ha (A, B, Sum, Carry) :
 xor(A,B,Sum),
 and(A, B, Carry) .
hs (A, B, Diff, Borrow) :
 xor(A, B, Diff),
 not (A, A_not),
 and (A_not, B, Borrow) .
fa(A,B,Cin,S,Cout) :
 xor(A,B,X), 
 xor(X,Cin,S),
 and(X,Cin,Y),
 or(Y,Z,Cout).
and(0,0,0).
and(0,1,0).
and(l,l,l).
and(1,0,0).
xor(0,0,0). 
xor(0,1,1).
xor(1,0,1).
xor(1,1,0).
not(0, 1) .
not(1,0). 
or(0,1 1).
or(1,0 1).
or(0,0 0).
or(l,1 1).

```

### Output:
![image](https://github.com/user-attachments/assets/f17b6319-1ad3-4660-a4d8-1488cb734f2b)
![image](https://github.com/user-attachments/assets/35e96c68-d3be-4926-8d8d-4cd9d447831b)
![image](https://github.com/user-attachments/assets/ea4d23e9-c3a5-4b31-81bc-4bd4e38db411)
![image](https://github.com/user-attachments/assets/4f85ec44-1656-4983-a3b9-cccbfa335888)



### Result:
Thus the truth table of circuit verified sucessfully.
