# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to create an inner class and access it from the outer class.

## AIM:
To write a Java program to create an inner class and access it from the outer class.

## ALGORITHM :
1. Create an Outer class.
2. Inside it, create a non-static Inner class.
3. Add a method inside the inner class that prints a message.
4. Create an object of the outer class.
5. Use the outer class object to create an object of the inner class.
6. Call the inner class method using the inner class object.
7. Execute the program.

## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122
*/
```

## SOURCE CODE:
```
import java.util.*;

class Outer {
    class Inner {
        void showMessage(String name){
            System.out.println("Hello, " + name + "! This message is from the Inner Class.");
        }
    }
}

public class Main {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        Outer outer = new Outer();
        Outer.Inner inner = outer.new Inner();
        inner.showMessage(name);
        
    }
}

```

## OUTPUT:
<img width="1165" height="377" alt="image (16)" src="https://github.com/user-attachments/assets/e4d64105-3e32-4ae0-a053-7450ceefa003" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
