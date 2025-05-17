# Ex.No:12(A)         JAVA TREE MAP
## AIM:
 To implement a Java program to associate the specified value with the specified key in a Tree Map.

## ALGORITHM :

1.	Start the Program
2.	Import `java.util.*` and `java.util.Map.Entry`
3.	Define `Example6` class with `main` method:
-	a) Initialize `TreeMap<String, String> tree_map1`
-	b) Read integer `size` for entries count.
4.	Use a loop to:
-	a) Read `String` values `n1` and `s1`
-	b) Insert each pair into `tree_map1`
5.	Print `tree_map1` as `"Original TreeMap content: "`
6.	Define `sort_key` class that implements `Comparator<String>`:
-	Override `compare` method to compare `String` values `str1` and `str2` using
`compareTo`
7.	End



## PROGRAM:
 ```
Program to implement a JAVA TREE MAP using Java
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
        TreeMap<Integer, String> map = new TreeMap<>(Comparator.naturalOrder());
        int n = sn.nextInt();
        for(int i=0; i<n; i++)
        {
            map.put(sn.nextInt(), sn.next());
        }
        System.out.println("Orginal TreeMap content: " + map);
    }
}

```






## OUTPUT:

![Screenshot 2025-05-17 180947](https://github.com/user-attachments/assets/b6edfd80-db1f-4b72-b4d5-3b66caaeb635)


## RESULT:
Thus the Java program to associate the specified value with the specified key in a Tree Map was executed successfully.
