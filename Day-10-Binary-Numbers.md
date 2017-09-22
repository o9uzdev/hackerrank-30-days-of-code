# Day 10: Binary Numbers

https://www.hackerrank.com/challenges/30-binary-numbers

```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        in.close();

        char[] ch = Integer.toBinaryString(n).toCharArray();
        int syc = 0, max = 0;
        for (int i=0; i<ch.length; i++) {

            if(ch[i] == '1')
                syc++;

            if(syc > max)
                max = syc;

            if(ch[i] == '0')
                syc = 0;
        }
        System.out.println(max);
    }
}
```