# Day 1: Data Types

https://www.hackerrank.com/challenges/30-data-types

```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {
	
    public static void main(String[] args) {
      int i = 4;
      double d = 4.0;
      String s = "HackerRank ";

      Scanner scan = new Scanner(System.in);
      /* Declare second integer, double, and String variables. */
      int tamSayi;
      double ondalikliSayi;
      String metin;
      /* Read and save an integer, double, and String to your variables.*/
      // Note: If you have trouble reading the entire String, please go back and review the Tutorial closely.
      tamSayi = scan.nextInt();
      ondalikliSayi = scan.nextDouble();
      scan.nextLine();
      metin = scan.nextLine();
      /* Print the sum of both integer variables on a new line. */
      System.out.println(i + tamSayi);
      System.out.println(d + ondalikliSayi);
      /* Print the sum of the double variables on a new line. */
      System.out.println(s + metin);
      /* Concatenate and print the String variables on a new line; 
        the 's' variable above should be printed first. */
      scan.close();
    }
}
```