# Day 6: Let's Review

https://www.hackerrank.com/challenges/30-review-loop

```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();
        sc.nextLine();
        String[] words = new String[t];
        
        for( int i=0; i <= t-1; i++ ) {
            words[i] = sc.nextLine();
        }
        sc.close();
        
        for( int i=0; i <= t-1; i++ ) {
            char[] kelime = words[i].toCharArray();
            String tek = "";
            String cift = "";

            for( int j=0; j < words[i].length(); j++ ) {
                if(j % 2 == 0) {
                    cift = cift + kelime[j];
                } else {
                    tek = tek + kelime[j];
                }
            }
            System.out.printf("%s %s\n", cift, tek);
        }
    }
}
```