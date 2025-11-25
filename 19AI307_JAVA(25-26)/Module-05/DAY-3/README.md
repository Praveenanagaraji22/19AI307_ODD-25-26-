# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
Write a program to count the number of words in a file.

## AIM:
To write a Java program that reads a text file and counts the number of words present in the file using file handling mechanisms.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a File object to reference the input text file.
4. Use Scanner or FileReader to read the contents of the file.
5. Split the file content into words using space or delimiter.
6. Count the total number of words.
7. Display the word count.
8. End the program.

## PROGRAM:
 ```
Program to implement a File Handling using Java
Developed by: PRAVEENA N
Register Number: 212222040122
```

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

public class WordCountInFile {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        try {
            String content = sc.nextLine();
            FileWriter fw = new FileWriter("input.txt");
            fw.write(content);
            fw.close();
            BufferedReader br = new BufferedReader(new FileReader("input.txt"));
            String line;
            int wordCount = 0;
            while ((line = br.readLine()) != null) {
                String[] words = line.trim().split("\\s+");
                if (!line.trim().isEmpty()) {
                    wordCount += words.length;
                }
            }

            br.close();
            System.out.println("Number of words in the file: " + wordCount);

        }
        catch (IOException e) {
            System.out.println("Error: " + e.getMessage());
        }
        finally {
            sc.close();
        }
    }
}
```

## OUTPUT:
<img width="1071" height="251" alt="image" src="https://github.com/user-attachments/assets/dc882d7a-9164-4532-8790-9fed1e52a225" />

## RESULT:
The program was implemented successfully and verified.

