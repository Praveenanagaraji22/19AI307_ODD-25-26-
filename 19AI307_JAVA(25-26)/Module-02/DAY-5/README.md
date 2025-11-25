# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Write a method that accepts a string and returns whether it contains only lowercase letters or not.

## AIM:
To write a method that accepts a string and returns whether it contains only lowercase letters or not.

## ALGORITHM :
1.	Start the program.
2.	Pass the string to the method isAllLowercase().
3.	Inside the method, loop through each character of the string.
4.	For each character, check if it is not lowercase; if found, return false.
5.	If the loop finishes without finding any uppercase or non-lowercase characters, return true and display the resul


## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: PRAVEENA N
RegisterNumber:  212222040122
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class prog {
    public static boolean isAllLowercase(String input) {
        for(int i=0;i<input.length();i++){
            if(!Character.isLowerCase(input.charAt(i))){
                return false;
            }
        }
        return true;
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String str = scanner.nextLine();
        // Call the method and display result
        System.out.print(isAllLowercase(str));
        scanner.close();
    }
}
```

## OUTPUT:
<img width="956" height="353" alt="Screenshot 2025-11-23 084821" src="https://github.com/user-attachments/assets/1d66d2fd-4dce-4c87-abb5-f421e0ad3b70" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
