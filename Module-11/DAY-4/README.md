# Ex.No:11(D) RELATED TO MAP CONCEPTS

## AIM:
To Create a java program to insert and display the key and values using map interface.

## ALGORITHM :

1.	Start
2.	Import `java.util.*`
3.	Define class `Deivamagal` with `main` method:
-	a) Read integer `n` (number of entries).
-	b) Create a `HashMap` `hash`.
4.	Loop to read key-value pairs and add to `hash`.
5.	Print `"Map: " + hash`, keys, values, and entries.
6.	End




## PROGRAM:
 ```
Program to implement a RELATED TO MAP CONCEPTS using Java
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
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        Map<Integer,String> hash=new HashMap<>(); 
        
        for(int i=0; i<n; i++)
        {
            hash.put(sc.nextInt(),sc.next());
        }
        
        System.out.println("Map: " + hash); 
        System.out.println("Keys: " + hash.keySet()); 
        System.out.println("Values: " + hash.values());
        System.out.println("Entries: " + hash.entrySet());
    }
}

```






## OUTPUT:

![Screenshot 2025-05-17 180155](https://github.com/user-attachments/assets/3266f510-9a70-463d-bf1d-cf533d6e52a2)


## RESULT:
Thus the java program to insert and display the key and values using map interface was  executed and verified successfully.


