# Ex.No: 5   Logic Programming – Factorial of number   
### DATE: 19/03/2025                                                                          
### REGISTER NUMBER : 212222060311
### AIM: 
To  write  a logic program for finding the factorial of given number using SWI-PROLOG. 
### Algorithm:
1. STEP 1: Start the program
2. STEP 2:  Write a rules for finding factorial of given program in SWI-PROLOG.
3.   a)	factorial of 0 is 1 => written as factorial(0,1).
4.   b)	factorial of number greater than 0 obtained by recursively calling the factorial    function.
5. STEP 3: Run the program  to find answer of  query.
6. STEP 4: Stop the program.

### Program:

```

fact(N,Res):-
    N>0,
    N1 is N-1,
    fact(N1,Res1),
    Res is N*Res1.
fact(0,1).


```



### Output:

![Screenshot 2025-03-19 112317](https://github.com/user-attachments/assets/f7a28a06-9271-4c6f-b7f5-5162ecedfe30)



### Result:
Thus the factorial of given number was found by logic programming. 
