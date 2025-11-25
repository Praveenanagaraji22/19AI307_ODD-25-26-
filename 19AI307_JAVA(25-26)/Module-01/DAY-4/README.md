# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java Program to count Even and Odd Numbers in an Array.

## AIM:
To write a Java program that takes an array of integers from the user and counts how many of them are even and how many are odd.

## ALGORITHM :
1. Start
2. Read the size of the array n.
3. Declare an integer array of size n.
4. Read all n integers from the user and store them in the array.
5. Initialize two counters:
        evenCount = 0, oddCount = 0
6. Traverse the array:
7. If element % 2 == 0, increment evenCount
   Else, increment oddCount
8. Print the values of evenCount and oddCount.
9. End.

## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
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
      int num = sc .nextInt();
      int[] arr = new int[num];
      for(int i =0;i<num;i++)
      {
          arr[i]= sc.nextInt();
      }
      int count=0,oddcount=0;
      for(int i=0;i<num;i++){
      if(arr[i]%2==0)
      {
          count++;
      }
      else if(arr[i]%2!=0)
      {
          oddcount++;
      }
      }
      System.out.println("Number of even elements: "+count);
      System.out.println("Number of odd elements: "+oddcount);
      
    }
}
```

## OUTPUT:
<img width="599" height="583" alt="image (6)" src="https://github.com/user-attachments/assets/dcb8e413-4b4a-410a-8261-399cbcf05c05" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

