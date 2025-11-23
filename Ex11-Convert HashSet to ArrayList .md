# Ex11 Convert HashSet to ArrayList in Java
## DATE:22-09-2025
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1. Start the program.  
2. Create a `HashSet` and add distinct integer elements to it.  
3. Use the `ArrayList` constructor to convert the `HashSet` into an `ArrayList`.  
4. Display the elements of both the `HashSet` and the `ArrayList`.  
5. Stop the program.   
   

## Program:
```java
/*
Program to To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: K L RAVEENDRANATH
RegisterNumber:  212224060212
*/
import java.util.*;

public class HashSetToArrayList {

    public static ArrayList<Integer> convertToArrayList(HashSet<Integer> set) {
        // Type Your Code Here.
        return new ArrayList<>(set);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            set.add(num);
        }

        ArrayList<Integer> list = convertToArrayList(set);
        System.out.println("ArrayList contents:");
        for (int num : list) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}
```

## Output:
<img width="604" height="646" alt="image" src="https://github.com/user-attachments/assets/2ef72d26-2656-4772-9ef5-2a6efa8357e5" />

## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
