# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE:25-09-2025
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1. Start the program.    
2. Create a `LinkedHashMap` to store numbers and their frequency counts.    
3. For each incoming number in the stream:    
   - Increment its count in the map.    
4. Iterate through the map to find the first number with a count of 1.    
5. Display the first unique number.    
6. Stop the program.    
   

## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: K L RAVEENDRANATH
RegisterNumber:  212224060212
*/

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
```

## Output:
<img width="786" height="589" alt="image" src="https://github.com/user-attachments/assets/adfd5f62-3778-4a2a-8d6b-bd8db3fc5a23" />




## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
