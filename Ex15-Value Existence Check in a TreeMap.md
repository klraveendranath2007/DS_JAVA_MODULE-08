# Ex15 Value Existence Check in a TreeMap
## DATE:
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

public class TreeMapValueCheck {
    public static void main(String[] args) {
        TreeMap<Integer, String> map = new TreeMap<>();
        map.put(1, "Apple");
        map.put(2, "Banana");
        map.put(3, "Cherry");
        map.put(4, "Mango");

        System.out.println("TreeMap: " + map);
        String valueToCheck = "Grapes";

        if (map.containsValue(valueToCheck))
            System.out.println("The value '" + valueToCheck + "' exists in the TreeMap.");
        else
            System.out.println("The value '" + valueToCheck + "' does not exist in the TreeMap.");
    }
}

```

## Output:
<img width="476" height="153" alt="image" src="https://github.com/user-attachments/assets/df275fff-989e-42d0-8296-15adb68c3c9d" />


## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
