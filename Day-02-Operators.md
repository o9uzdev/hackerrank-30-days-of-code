# Day 2: Operators

https://www.hackerrank.com/challenges/30-operators

```java
import java.util.*;
import java.math.*;

public class Arithmetic {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        double mealCost = scan.nextDouble(); // original meal price
        int tipPercent = scan.nextInt(); // tip percentage
        int taxPercent = scan.nextInt(); // tax percentage
        scan.close();
        double tip, tax, myTotalCost;

        // Write your calculation code here.
        tip = mealCost * tipPercent / 100;
        tax = mealCost * taxPercent / 100;
        myTotalCost = mealCost + tip + tax;
        
        // cast the result of the rounding operation to an int and save it as totalCost 
        int totalCost = (int) Math.round(myTotalCost);

        // Print your result
        System.out.printf("The total meal cost is %d dollars.", totalCost);
    }
}
```