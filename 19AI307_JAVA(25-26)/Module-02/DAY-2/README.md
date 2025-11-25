# Ex.No:2(B) METHODS

## QUESTION:
Write a class with one static method and one non-static method. Call both from the main() method.
When staticMethod() is called, it should print  "I am static".
When nonStaticMethod() is called, it should print  "I am non-static".

## AIM:
To write a Java program that contains a class with one static method and one non-static method, and call both methods from the main() method.

## ALGORITHM :
1. Start
2. Create a class.
3. Inside the class, define a static method named staticMethod() that prints "I am static".
4. Define a non-static method named nonStaticMethod() that prints "I am non-static".
5. In the main() method: Call the static method directly using the class name.
6. Create an object of the class.
7. Using that object, call the non-static method.
8. End

## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main {
    static void staticMethod() {
        System.out.println("I am static");
    }
    void nonStaticMethod() {
        System.out.println("I am non-static");
    }
    public static void main(String[] args) {
        staticMethod();
        Main obj = new Main();
        obj.nonStaticMethod();
    }
}

```

## OUTPUT:
<img width="459" height="282" alt="image (11)" src="https://github.com/user-attachments/assets/0334cf95-4a89-41df-8a38-79ec673ebb39" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
