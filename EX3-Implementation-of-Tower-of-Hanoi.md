EX3 Implementation of Tower of Hanoi
DATE:
AIM:
To write a C program to implement Tower of Hanoi

Algorithm
Start the program.
Check if n is greater than 0.
Recursively move n-1 disks from source (x) to auxiliary (z) using destination (y).
Print the move of the n-th disk from source (x) to destination (y).
Recursively move n-1 disks from auxiliary (z) to destination (y) using source (x).
The function is called initially with TOH(n, 'A', 'B', 'C') where 'A', 'B', and 'C' are the rods.
End
Program:
/*
Program to implement Tower of Hanoi
Developed by: RAJARAMAN V
RegisterNumber:  212223110038
*/
```
#include<stdio.h> 
void TOH(int n,char x,char y,char z) 
{ 
if(n>0) 
{ 
TOH(n-1,x,z,y); 
printf("%c to %c",x,y); 
printf("\n"); 
TOH(n-1,z,y,x); 
} 
} 
int main() 
{ 
int n=2; 
TOH(n,'A','B','C'); 
}
```
Output:
![image](https://github.com/user-attachments/assets/55038056-20f0-4474-909d-b692b5928306)


Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
