# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE:26-11-2025
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm:
1. Start the program.
2. Read an integer n (the number of inputs in the stream).
3. Create an empty LinkedHashMap<Integer, Integer> named map.
4. Repeat the following steps for each of the n numbers.
5. After processing all numbers, end the program.
## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: VEDHASHREE G
RegisterNumber:  212223240171

import java.util.*;

public class FirstUniqueNumberStream {

    public static void processStream(int n, Scanner sc) {
        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            map.put(num, map.getOrDefault(num, 0) + 1);
            boolean found = false;
            for (Map.Entry<Integer, Integer> entry : map.entrySet()) {
                if (entry.getValue() == 1) {
                    System.out.println("First unique number: " + entry.getKey());
                    found = true;
                    break;
                }
            }
            if (!found) {
                System.out.println("No unique number");
            }
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        processStream(n, sc);
        sc.close();
    }
}
*/
```

## Output:
<img width="864" height="610" alt="image" src="https://github.com/user-attachments/assets/2b44741c-fc76-4cd8-95d3-62025db5d7cf" />

## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
