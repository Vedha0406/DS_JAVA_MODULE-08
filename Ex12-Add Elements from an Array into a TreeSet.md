# Ex12 Add Elements from an Array into a TreeSet
## DATE: 26-11-2025
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Read input array
2. Create empty TreeSet
3. Insert all array elements into TreeSet
4. Print TreeSet elements (in sorted order)
## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: VEDHASHREE G
RegisterNumber:  212223240171

import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        // Type Your Code Here.
        TreeSet<Integer> set = new TreeSet<>();
        for (int a:arr)
            set.add(a);
        return set;

    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}

*/
```

## Output:
<img width="735" height="621" alt="image" src="https://github.com/user-attachments/assets/1da8d446-b317-4dba-b2d1-5e0eb094da37" />

## Result:
The program successfully adds elements from an array into a TreeSet.
