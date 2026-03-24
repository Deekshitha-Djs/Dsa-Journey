#Finding the Minimum and Maximum in an Array

##🧠Approach:  
-Traverse the array  
-Track min and max  

##🧾Code (java)

```java
public class MinMaxMatrix {
    public static void main(String[] args) {
        int[][] arr = {
            {3, 5, 1},
            {9, 2, 8}
        };

        int min = arr[0][0];
        int max = arr[0][0];

        for (int i = 0; i < arr.length; i++) {
            for (int j = 0; j < arr[0].length; j++) {
                if (arr[i][j] < min) {
                    min = arr[i][j];
                }
                if (arr[i][j] > max) {
                    max = arr[i][j];
                }
            }
        }

        System.out.println("Min: " + min);
        System.out.println("Max: " + max);
    }
}
```
##⏱️ Complexity  
-Time: O(m*n)  
-Space: O(1)  

##✨ Key Takeaways  
-Basic array traversal  
-Important foundation problem  
