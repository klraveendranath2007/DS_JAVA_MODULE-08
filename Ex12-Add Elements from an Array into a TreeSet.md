# Ex12 Add Elements from an Array into a TreeSet
## DATE:22-09-2025
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Start the program.    
2. Initialize an array with integer elements.    
3. Create an empty `TreeSet`.    
4. Add all elements from the array into the `TreeSet`.    
5. Display the elements of the `TreeSet` (which are automatically sorted).    
6. Stop the program.   

## Program:
```java
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: K L RAVEENDRANATH
RegisterNumber: 212224060212 
*/
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        
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

Output:

```

## Output:
<img width="724" height="504" alt="image" src="https://github.com/user-attachments/assets/af1e1a04-a777-43e2-97a0-258d19c4a4d5" />



## Result:
The program successfully adds elements from an array into a TreeSet.
