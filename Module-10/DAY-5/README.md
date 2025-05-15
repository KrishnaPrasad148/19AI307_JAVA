# Ex.No:10(E)  JAVA LINKEDHASH SET

## AIM:
To write a Java program using LinkedHashSet to store unique elements in insertion order, display all elements, and show the total size of the set.
## ALGORITHM :
a.	Import java.util.LinkedHashSet.
b.	Create a LinkedHashSet of type String.
c.	Add some elements using .add() method.
d.	Print all the elements in the set using a loop.
e.	Use .size() method to get and print the number of elements in the set.



## PROGRAM:
 ```
Program to implement a LINKEDHASH SET
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
        LinkedHashSet<String> hs = new LinkedHashSet<>();
        Scanner sn = new Scanner(System.in);
        int n = sn.nextInt();
        for(int i=0; i<n; i++)
        {
            hs.add(sn.next());
        }
        
        System.out.println("LinkedHashSet: " +hs);  
        System.out.println("The size of the set is: " + hs.size());  
    }
}

```






## OUTPUT:

![Screenshot 2025-05-15 112501](https://github.com/user-attachments/assets/edcca0ca-c3ea-4dad-82e8-3032b5ff8ccf)


## RESULT:

Thus the java program was successfully uses LinkedHashSet to store and display elements while maintaining insertion order and ensuring uniqueness. It also shows the correct count of unique elements. 
