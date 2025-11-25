# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to print the Fibonacci series using a for loop. The series starts with 0 and 1, and the next number is the sum of the previous two.

## AIM:
To write a Java program that prints the Fibonacci series using a for loop, starting from 0 and 1, where every next number is the sum of the previous two.

## ALGORITHM :
1. Start
2. Read the number of terms n to be printed.
3. Initialize:
     a = 0 (first term),b = 1 (second term)
4. Print a and b.
5. Loop from i = 2 to n - 1:
6. Compute c = a + b
7. Print c
8. Update values:
      a = b,b = c
9. End.

## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
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
        int num = sc.nextInt();
        int a=0, b=1;
        System.out.print("Fibonacci Series: ");
        if(num==1){
            System.out.print(a+" "+b);
        }else{
        for(int i=0;i<num;i++){
            System.out.print(a+" ");
            int temp=a+b;
            a=b;
            b=temp;
        }
        }
    }
}
```

## OUTPUT:
<img width="857" height="374" alt="image (5)" src="https://github.com/user-attachments/assets/b8e99449-6e04-4abe-beed-3260834236c4" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
