# Ex.No:3(D)    INTERFACE 

## QUESTION:
Two types of traffic controllers decide whether a vehicle can pass based on signal color. The decision logic varies by controller.AggressiveController: Allows only if "GREEN". DefensiveController: Allows for "GREEN" or "YELLOW"

## AIM:
To design two traffic controller classes where each decides if a vehicle can pass based on the signal color—AggressiveController allowing only GREEN, and DefensiveController allowing GREEN or YELLOW.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3. Define an interface TrafficController with the method canPass().
4. Create AggressiveController that returns true only when the signal is GREEN.
5. In main, based on controller type, create either an AggressiveController or DefensiveController object.
6. Call the canPass() method to check if the vehicle is allowed to go.
7. Print GO if true, otherwise print STOP, and end the program.

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: PRAVEENA N
RegisterNumber:  212222040122
*/
```

## SOURCE CODE:

```
import java.util.*;

interface TrafficController {
    boolean canPass(String signalColor);
}

class AggressiveController implements TrafficController {
    public boolean canPass(String signalColor) {
        return signalColor.equalsIgnoreCase("GREEN");
    }
}

class DefensiveController implements TrafficController {
    public boolean canPass(String signalColor) {
        return signalColor.equalsIgnoreCase("GREEN") || signalColor.equalsIgnoreCase("YELLOW");
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String signalColor = sc.next();
        int controllerType = sc.nextInt();
        sc.close();
        
        TrafficController controller;
        
        if (controllerType == 1)
            controller = new AggressiveController();
        else
            controller = new DefensiveController();
        
        if (controller.canPass(signalColor))
            System.out.println("GO");
        else
            System.out.println("STOP");
    }
}
```



## OUTPUT:

<img width="1102" height="339" alt="image" src="https://github.com/user-attachments/assets/e63baf57-8f86-4458-9aff-e8a4d4f142d0" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
