# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely has mastered printing in Java, and now she wants to learn how arithmetic operators work. She’s curious about how Java can add, subtract, multiply, divide, and find remainders of two numbers.

Write a Java program that:
Accepts two integer numbers from the user.
Demonstrates all 5 arithmetic operations:
Addition (+)
Subtraction (-)
Multiplication (*)
Division (/)
Modulus (%)
Displays the result of each operation in a separate line with a clear message.

Input Format
First line: Integer → first number
Second line: Integer → second number

Output Format
Each line shows the result of an arithmetic operation in this format:


Sum = <value>
Difference = <value>
Product = <value>
Quotient = <value>
Remainder = <value>
Ensure integer division and modulus are correctly handled. Assume the second number will not be 0.

## AIM:
To write a Java program that accepts two integer inputs from the user and performs all five arithmetic operations— addition, subtraction, multiplication, division, and modulus—and displays the results clearly on separate lines.

## ALGORITHM :
1.	Start
2. Declare two integer variables a and b.
3. Read the first integer from the user and store it in variable a.
4. Read the second integer from the user and store it in variable b (given that b ≠ 0).
5. Perform arithmetic operations:
   Compute sum = a + b,
   Compute difference = a - b,
   Compute product = a * b,
   Compute quotient = a / b (integer division),
   Compute remainder = a % b.

6. Display all results in the required format:
   "Sum = <value>"
   "Difference = <value>"
   "Product = <value>"
   "Quotient = <value>"
   "Remainder = <value>"
7. End

## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122
*/
```

## Sourcecode.java:
```
import java.util.*;
class prog{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int num1 = sc.nextInt();
        int num2 = sc.nextInt();
        int num3 = num1+num2;
        System.out.println("Sum = "+num3);
        int num4=num1-num2;
        System.out.println("Difference = "+num4);
        int num5=num1*num2;
        System.out.println("Product = "+num5);
        int num6= num1/num2;
        System.out.println("Quotient = "+num6);
        int num7=num1%num2;
        System.out.println("Remainder = "+num7);
        
    }
}
```

## OUTPUT:
<img width="427" height="248" alt="image (5)" src="https://github.com/user-attachments/assets/fbe6d17c-9351-488f-9c7b-cbad174a4101" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
