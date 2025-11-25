# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
In a magical building, an elevator behaves oddly:
If the floor number is divisible by 3 and 5, it says "Skipped".
If the floor number is divisible by 3 only, it says "Beware!".
If the floor number is divisible by 5 only, it says "Blessings!".
Otherwise, it announces the floor number - print - "Floor {number}" .

Write a Java program to simulate this elevator logic for a given floor number.

## AIM:
To write a Java program that takes a floor number as input and displays a special message based on divisibility rules.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util.*'.
3.	Read an integer input from the user and store it in a variable floor.
4.	Check conditions in the correct order:
If floor % 3 == 0 and floor % 5 == 0
→ Print "Skipped"
Else if floor % 3 == 0
→ Print "Beware!"
Else if floor % 5 == 0
→ Print "Blessings!"
Else
→ Print "Floor " + floor
5. End

## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int num=sc.nextInt();
        if(num%3==0 && num%5==0)
        {
            System.out.print("Skipped");
        }
        else if(num%3==0)
        {
            System.out.print("Beware!");
        }
        else if(num%5==0)
        {
            System.out.print("Blessings!");
        }
        else
        {
            System.out.print("Floor "+num);
        }
    }
}
```

## OUTPUT:
<img width="382" height="332" alt="image (8)" src="https://github.com/user-attachments/assets/91d48a91-49d1-403c-8ace-a3e8e9b6ee09" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
