# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to calculate the power of a given number.

## AIM:
To write a Java program to calculate the power of a given number.

## ALGORITHM :
1. Start
2. Read two integers from the user:Base number, Exponent.
3. Initialize result = 1.
4. Repeat a loop exponent times: Multiply result = result * base.
5. After the loop ends, print the final result.
6. End.

## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122 
*/
```

## SOURCE CODE:
```
import java.util.*;
import java.lang.*;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int num1 = sc.nextInt();
        int num2 = sc.nextInt();
        float res= (float)Math.pow(num1,num2);
        System.out.print((float)num1+" raised to the power of "+(float)num2+" is: "+res);
    }
}
```

## OUTPUT:
<img width="1000" height="353" alt="image (7)" src="https://github.com/user-attachments/assets/830ad3a8-5b71-43bc-95b0-4bdf5ed7b8c5" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
