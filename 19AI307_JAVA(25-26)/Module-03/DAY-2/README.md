# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program to create a class MaxFinder with three overloaded max() methods:
max(int a, int b) – returns the maximum of two integers.
max(double a, double b) – returns the maximum of two double values.
max(int a, int b, int c) – returns the maximum of three integers.
In the main() method, demonstrate the use of each overloaded method with various inputs.

## AIM:
To create a Java class MaxFinder that contains three overloaded max() methods to find the maximum.

## ALGORITHM :
1. Start the program.
2. Create a class MaxFinder.
3. Define the following overloaded methods: max(int a, int b) – returns the greater of two integers, max(double a, double b) – returns the greater of two double values, max(int a, int b, int c) – returns the greatest of three integers.
4. Create a main() method in the class.
5. Call each overloaded method with sample values.
6. Print the results.
7. End the program.

## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class MaxFinder {

    public int max(int a, int b) {
        return (a > b) ? a : b;
    }

    public double max(double a, double b) {
        return (a > b) ? a : b;
    }

    public int max(int a, int b, int c) {
        return (a > b && a > c) ? a : (b > c ? b : c);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        MaxFinder mf = new MaxFinder();

        int a1 = sc.nextInt();
        int b1 = sc.nextInt();
        double a2 = sc.nextDouble();
        double b2 = sc.nextDouble();
        int a3 = sc.nextInt();
        int b3 = sc.nextInt();
        int c3 = sc.nextInt();

        System.out.println("Max(" + a1 + ", " + b1 + "): " + mf.max(a1, b1));
        System.out.println("Max(" + a2 + ", " + b2 + "): " + mf.max(a2, b2));
        System.out.println("Max(" + a3 + ", " + b3 + ", " + c3 + "): " + mf.max(a3, b3, c3));

    }
}
```

## OUTPUT:
<img width="586" height="429" alt="image (14)" src="https://github.com/user-attachments/assets/9e99e0eb-b4d7-4980-80cf-23701f7ab66d" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

