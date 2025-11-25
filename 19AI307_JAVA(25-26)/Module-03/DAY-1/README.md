# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
A food delivery application manages and processes food orders made by two categories of users: NormalUser and PrimeUser. Each food order contains basic information such as an order ID, the customer's name, the cost of the ordered items (referred to as the total amount), and the delivery charge applied to that order.
You are required to implement this system using the concept of inheritance in object-oriented programming.
The base class is called Order. It includes the following attributes:
orderId – a string representing the unique identifier for the order
customerName – a string containing the name of the person who placed the order
totalAmount – a double value representing the total cost of the food items
deliveryCharge – a double value representing the delivery fee applied to the order
From the Order class, two derived classes are created:
NormalUser:
This class represents customers who do not have any delivery benefits. For NormalUser, the final amount they need to pay is the total food cost plus the full delivery charge. The formula is:
finalAmount = totalAmount + deliveryCharge
PrimeUser:
Prime users receive a 50% discount on the delivery charge. Their final payable amount is calculated as:
finalAmount = totalAmount + (deliveryCharge × 0.5)
Your task is to develop a program that:
Accepts exactly three food order inputs from the user.
Each input begins with the user type, either "Normal" or "Prime", followed by order ID, customer name, total food amount, and delivery charge.
Depending on the user type, the final amount is calculated using the appropriate formula.
For each order, the program should display the full details including the user type and final payable amount.
```
import java.util.Scanner;
import java.text.DecimalFormat;

class Order {
    String orderId;
    String customerName;
    double totalAmount;
    double deliveryCharge;

    public Order(String orderId, String customerName, double totalAmount, double deliveryCharge) {
        this.orderId = orderId;
        this.customerName = customerName;
        this.totalAmount = totalAmount;
        this.deliveryCharge = deliveryCharge;
    }

    double calculateFinalAmount() {
        return totalAmount + deliveryCharge;
    }

    void display(String userType) {
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Order ID: " + orderId);
        System.out.println("Customer Name: " + customerName);
        System.out.println("User Type: " + userType);
        System.out.println("Total Amount: " + totalAmount);
        System.out.println("Delivery Charge: " + deliveryCharge);
        System.out.println("Final Amount: " + df.format(calculateFinalAmount()));
        
    }
}
//Continue your code here
```

## AIM:
To develop a Java program using inheritance to manage food orders for two types of users—NormalUser and PrimeUser. The program should read three orders, calculate the final payable amount based on user type, and display the complete order details.

## ALGORITHM :
1. Start
2. Create a base class Order with attributes: OrderId, customerName, totalAmount, deliveryCharge
3. Implement a method calculateFinalAmount() in Order that returns totalAmount + deliveryCharge.
4. Create two subclasses: NormalUser: uses full delivery charge, PrimeUser: uses 50% delivery charge.
5. Override calculateFinalAmount() in both subclasses according to:
Normal: totalAmount + deliveryCharge
Prime: totalAmount + (deliveryCharge × 0.5)
6. In main, read exactly 3 orders.
7. Based on user type ("Normal" or "Prime"): Create the respective object, Calculate final amount, Display all order details
8. End.

## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: PRAVEENA N
RegisterNumber: 212222040122 
*/
```

## SOURCE CODE:
```
import java.util.*;
import java.text.DecimalFormat;

class Order {
    String orderId;
    String customerName;
    double totalAmount;
    double deliveryCharge;

    public Order(String orderId, String customerName, double totalAmount, double deliveryCharge) {
        this.orderId = orderId;
        this.customerName = customerName;
        this.totalAmount = totalAmount;
        this.deliveryCharge = deliveryCharge;
    }

    double calculateFinalAmount() {
        return totalAmount + deliveryCharge;
    }

   void display(String userType) {
    DecimalFormat dfOne = new DecimalFormat("0.0");   // one decimal place
    DecimalFormat dfTwo = new DecimalFormat("0.00");  // two decimal places

    System.out.println("Order ID: " + orderId);
    System.out.println("Customer Name: " + customerName);
    System.out.println("User Type: " + userType);
    System.out.println("Total Amount: " + dfOne.format(totalAmount));
    System.out.println("Delivery Charge: " + dfOne.format(deliveryCharge));
    System.out.println("Final Amount: " + dfTwo.format(calculateFinalAmount()));
}


}

class NormalUser extends Order {
    public NormalUser(String orderId, String customerName, double totalAmount, double deliveryCharge) {
        super(orderId, customerName, totalAmount, deliveryCharge);
    }

    @Override
    double calculateFinalAmount() {
        return totalAmount + deliveryCharge;
    }
}

class PrimeUser extends Order {
    public PrimeUser(String orderId, String customerName, double totalAmount, double deliveryCharge) {
        super(orderId, customerName, totalAmount, deliveryCharge);
    }

    @Override
    double calculateFinalAmount() {
        return totalAmount + (deliveryCharge * 0.5);
    }
}

public class FoodOrderApp {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int orderCount = 0;
        while (sc.hasNextLine() && orderCount < 3) { // Stop after 3 orders or if input ends
            String userType = sc.nextLine().trim();
            if (!sc.hasNextLine()) break;
            String orderId = sc.nextLine().trim();
            if (!sc.hasNextLine()) break;
            String customerName = sc.nextLine().trim();
            if (!sc.hasNextLine()) break;
            double totalAmount = Double.parseDouble(sc.nextLine().trim());
            if (!sc.hasNextLine()) break;
            double deliveryCharge = Double.parseDouble(sc.nextLine().trim());

            if (userType.equalsIgnoreCase("Normal")) {
                NormalUser order = new NormalUser(orderId, customerName, totalAmount, deliveryCharge);
                order.display("Normal");
            } else if (userType.equalsIgnoreCase("Prime")) {
                PrimeUser order = new PrimeUser(orderId, customerName, totalAmount, deliveryCharge);
                order.display("Prime");
            } else {
                System.out.println("Invalid user type!");
            }

            System.out.println(); // Empty line between orders
            orderCount++;
        }

    }
}
```

## OUTPUT:
<img width="581" height="633" alt="image (13)" src="https://github.com/user-attachments/assets/94aa75a5-47a0-434c-abd1-1c18088c9d0f" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.

