# Ex.No:11(C)             JAVA LINKED HASHMAP
 ## AIM :

To Create a java program to display the contains key of 104 and to retrieve the key and value using linked hash map.

## ALGORITHM :

1.	Start the Program
2.	Import `java.util.*`
3.	Define class `A` with `main` method:
-	a) Initialize `Scanner` and read integer `n`
-	b) Create a `LinkedHashMap` named `hash` to store integer keys and string values
4.	Use a loop to:
-	a) Read an integer and string from the user
-	b) Add the integer as the key and the string as the value in `hash`
5.	Use an enhanced `for` loop to iterate through `hash` and print each key-value pair
6.	Check if the `hash` contains the key `104` and print the result
7.	End


## PROGRAM:
 ```
Program to implement a JAVA LINKED HASH MAP using Java
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
        LinkedHashMap<Integer, String> map = new LinkedHashMap<>();
        int size = sn.nextInt();
        for(int i=0; i<size; i++)
        {
            map.put(sn.nextInt(), sn.next());
        }
        for(int key : map.keySet())
        {
            System.out.println("key: " + key + " value: " + map.get(key));
        }
        System.out.println("Does HashMap contains 104 as key: " + hash.containsKey(104)) );
    }
}

```






## OUTPUT:

![Screenshot 2025-05-17 175758](https://github.com/user-attachments/assets/a62279a2-f274-4c45-a6f4-2160b3c063a3)


## RESULT:
Thus the  java program to display the contains key of 104 and to retrieve the key and value using linked hash map was executed successfully.








