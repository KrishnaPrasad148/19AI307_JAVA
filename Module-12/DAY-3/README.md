# Ex.No:12(C)             JAVA STACK & VECTOR
 ## AIM :

To Write a java program to create vector and read the elements for two vector in java collection.(Use equals method )
## ALGORITHM :

1.	Start the Program
2.	In `main`:
-	a) Create a `Scanner` object to read input.
-	b) Read an integer `n1` (the size of the first vector).
-	c) Initialize `Vector<String> vector1`.
-	d) Use a `for` loop to read `n1` strings and add each to `vector1`.
3.	Repeat similar steps for a second vector:
a)	Read an integer `n2` (size of the second vector).
b)	Initialize `Vector<String> vector2`.
c)	Use a `for` loop to read `n2` strings and add each to `vector2`.
4.	Use `equals()` to compare `vector1` and `vector2` and print whether they are equal.
5.	End.



## PROGRAM:
 ```
Program to implement a JAVA STACK & VECTOR  using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

public class Main
{
    public static void main(String args[])
    {
        Scanner sn = new Scanner(System.in);
        
        int n = sn.nextInt();
        sn.nextLine();
        Vector<Object> vec1 = new Vector<>();
        for(int i=0; i<n; i++)
        {
            vec1.add(sn.next());
        }
        System.out.println("The vector is: " + vec1);
        
        int m = sn.nextInt();
        sn.nextLine();
        Vector<Object> vec2 = new Vector<>();
        for(int i=0; i<m; i++)
        {
            vec2.add(sn.next());
        }
        System.out.println("The Vector is: " + vec2);
        
        System.out.println("Are both of them equal? " + vec1.equals(vec2));
    }
}

```






## OUTPUT:

![Screenshot 2025-05-17 181403](https://github.com/user-attachments/assets/5dcabafa-0439-4bf5-b865-6233cf7a2eef)


## RESULT:

Thus the java program to create vector and read the elements for two vector in java collection.(Use equals method ) was executed successfully.








