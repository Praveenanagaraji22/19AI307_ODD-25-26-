# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Vehicle with attributes as number, type and owner.
<img width="503" height="144" alt="image (9)" src="https://github.com/user-attachments/assets/f6101c52-1afd-40dc-8f22-44cea4615353" />


## AIM:
To create a class Vehicle with attributes as number, type and owner.

## ALGORITHM :
1. Start
2. Create a class Vehicle with attributes: number, type, owner.
3. Create a Scanner object to read user input.
4. Create the first Vehicle object: Read and store number, type, and owner.
5. Create the second Vehicle object: Read and store number, type, and owner.
6. Print the details of both vehicles in the format: number | type | owner
7. Close the scanner
8. End	

## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class Vehicle
{
    String number;
    String type;
    String owner;
}
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Vehicle v1 = new Vehicle();
        v1.number = sc.next();
        v1.type = sc.next();
        v1.owner = sc.next();

        Vehicle v2 = new Vehicle();
        v2.number = sc.next();
        v2.type = sc.next();
        v2.owner = sc.next();

        System.out.println(v1.number + " | " + v1.type + " | " + v1.owner);
        System.out.println(v2.number + " | " + v2.type + " | " + v2.owner);

        sc.close();
    }
}

```

## OUTPUT:
<img width="503" height="144" alt="image (9)" src="https://github.com/user-attachments/assets/ef9dd14a-ff48-4efd-a390-d2b2c6f13465" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
