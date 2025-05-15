# Ex.No:10(A)         JAVA COLLECTION FRAMEWORK –ARRAY LIST
## AIM:
 To Create a Java Program to store n numbers (add elements of type Integer) and then display the n numbers using array List.

## ALGORITHM:
1.	Start the Program
2.	Import `java.util.*` for input handling and list functionality
3.	Define class `Snowdrop` with the `main` method:
-	a) Create `Scanner` object `sc` for input
-	b) Read an integer `n` to specify the number of elements
-	c) Create an `ArrayList` named `num` to store integers
4.	Use a `for` loop to:
-	a) Read `n` integers from input and add each to `num`
5.	Use an enhanced `for` loop to:
-	a) Iterate through `num` and print each element
6.	End

## PROGRAM:
 ```
Program to implement a ARRAY LIST using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*; 

public class Snowdrop
{
    public static void main(String args[])
    {
        Scanner sn = new Scanner(System.in); 
        int n = sn.nextInt();
        ArrayList<Integer> arr = new ArrayList<Integer>();
        
        for(int i=0; i<n; i++)
        {
            arr.add(sn.nextInt());
        }
        
        for(int i : arr)
        {
            System.out.println(i);
        }
    }
}

```






## OUTPUT:

![Screenshot 2025-05-15 110312](https://github.com/user-attachments/assets/ec85972a-84f4-41d0-89c8-41be3a267995)


## RESULT:
TThus the Java Program to store n numbers (add elements of type Integer) and then display the n numbers using array List was executed successfully.

