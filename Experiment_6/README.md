#AIM:
```java

import java.util.Scanner;

public class ArrayExceptionHandling {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Read size of array
        System.out.print("Enter size of the array: ");
        int n = sc.nextInt();

        int[] arr = new int[n];

        // Read array elements
        System.out.println("Enter " + n + " elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        // Read index to access
        System.out.print("Enter index to access (starting from 0): ");
        int index = sc.nextInt();

        try {
            // Attempt to access array element
            System.out.println("Element at index " + index + " is: " + arr[index]);
        } 
        catch (ArrayIndexOutOfBoundsException e) {
            // Handle invalid index
            System.out.println("Invalid index! Please enter index between 0 and " + (n - 1) + ".");
        }

        sc.close();
    }
}
```
#OUTPUT:()[!]


