# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Person with private instance variables name, age. and country. Provide public getter and setter methods to access and modify these variables.
```
public class Person {
  
    private String name;
    private int age;
    private String country;

   
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }

    
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }

    
    public String getCountry() {
        return country;
    }
    public void setCountry(String country) {
        this.country = country;
    }
}

Continue your code
```

## AIM:
To create a Java class Person with private instance variables (name, age, country) and provide public getter and setter methods to access and modify these variables.

## ALGORITHM :
1. Start
2. Create a class named Person.
3. Declare three private variables: name, age, and country.
4. Provide public getter and setter methods for each private variable.
5. In the main method: Create an object of the Person class.
6. Use setter methods to assign values to name, age, and country.
7. Use getter methods to retrieve and print the values.
8. End

## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class Person {
    private String name;
    private int age;
    private String country;

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }

    public String getCountry() {
        return country;
    }
    public void setCountry(String country) {
        this.country = country;
    }
}
public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Person p = new Person();
        p.setName(sc.nextLine());
        p.setAge(sc.nextInt());
        sc.nextLine(); 
        p.setCountry(sc.nextLine());
        System.out.println("Person 1");
        System.out.println("Name: " + p.getName());
        System.out.println("Age: " + p.getAge());
        System.out.println("Country: " + p.getCountry());
    }
}

```

## OUTPUT:
<img width="723" height="539" alt="image (12)" src="https://github.com/user-attachments/assets/06de92c5-4edc-4b1e-bd80-fd532af7dafc" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.


