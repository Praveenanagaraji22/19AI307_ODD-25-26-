# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Find the largest digit in a number using wrapper class methods.

## AIM:
To find the largest digit in a number using wrapper class methods.

## ALGORITHM :
1. Start the program.
2. Take an integer number.
3. Convert the number to a String using Integer.toString().
4. Traverse each character of the string.
5. Convert each character to a digit using Character.getNumericValue().
6. Compare and keep track of the largest digit.
7. Print the largest digit.
8. End the program.

## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class LargestDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        String str = Integer.toString(num);

        int largest = Integer.MIN_VALUE;

        for (int i = 0; i < str.length(); i++) {
            int digit = Character.getNumericValue(str.charAt(i));

            if (digit > largest) {
                largest = digit;
            }
        }

        System.out.println("The largest digit is: " + largest);
    }
}
```

## OUTPUT:
<img width="553" height="324" alt="image (15)" src="https://github.com/user-attachments/assets/d16e351a-d7c1-4309-b572-93ac4032e146" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

