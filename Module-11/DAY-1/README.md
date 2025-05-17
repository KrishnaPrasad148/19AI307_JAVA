# Ex.No:11(A)         JAVA TREESET
## AIM:
 To develop a Java program to iterate through all elements in a tree set.


## ALGORITHM :
1.	Start
2.	Import `java.util.*`
3.	Define class `Main` with `main` method:
-	a) Initialize `Scanner` and read integer `n`
-	b) Create a `TreeSet` named `set` to store integers in sorted order
4.	Use a loop to read `n` integers and add each to `set`
5.	Use an enhanced `for` loop to print each element in `set`
6.	End


## PROGRAM:
 ```
Program to implement a JAVA TREESET using Java
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
        TreeSet<Integer> treeset = new TreeSet<>();
        for(int i=0; i<n; i++)
        {
            treeset.add(sn.nextInt());
        }
        Iterator<Integer> itr = treeset.iterator();
        while(itr.hasNext())
        {
            System.out.println(itr.next());
        }
    }
}

```






## OUTPUT:

![Screenshot 2025-05-17 174744](https://github.com/user-attachments/assets/bfdf0b2f-5056-49c2-8360-671c97b7b075)


## RESULT:
Thus the java program to iterate through all elements in a tree set was executed successfully.

