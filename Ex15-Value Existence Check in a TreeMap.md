# Ex15 Value Existence Check in a TreeMap
## DATE:29-09-2025
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Start the program.    
2. Create a `TreeMap` and insert key–value pairs.    
3. Use the `containsValue()` method to check if a specific value exists in the map.    
4. Display whether the value is found or not.    
5. Stop the program.

## Program:
```java
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: K L RAVEENDRANATH
RegisterNumber:  212224060212
*/

import java.util.*;

public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        if (map.containsValue(searchValue)) {
            System.out.println("Value \"" + searchValue + "\" exists in the TreeMap.");
        } else {
            System.out.println("Value \"" + searchValue + "\" does not exist in the TreeMap.");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}

```

## Output:
<img width="1020" height="708" alt="image" src="https://github.com/user-attachments/assets/e32d32ab-93c4-4048-aef9-d3a16fa63cad" />



## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
