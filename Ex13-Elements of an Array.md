# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE:
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Start the program.    
2. Create an integer array of size 10.    
3. Use `Arrays.fill()` to assign a constant value to all 10 elements.    
4. Print the array elements using `Arrays.toString()`.    
5. End the program.     

## Program:
```java
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: K L RAVEENDRANATH
RegisterNumber: 212224060212
*/

import java.util.Arrays;

public class FillArray {
    public static void main(String[] args) {
        int[] arr = new int[10];
        Arrays.fill(arr, 5);
        System.out.println("Array after filling: " + Arrays.toString(arr));
    }
}
```

## Output:
<img width="512" height="133" alt="image" src="https://github.com/user-attachments/assets/3ff77a3d-818a-41a7-8a86-d69e72d9acc4" />


## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
