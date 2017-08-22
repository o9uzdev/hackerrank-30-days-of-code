# Day 5: Loops

https://www.hackerrank.com/challenges/30-loops

```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.close();

        for(int i = 1; i <= 10; i++){
            System.out.printf("%d x %d = %d\n", n, i, n*i);
        }
    }
}
```