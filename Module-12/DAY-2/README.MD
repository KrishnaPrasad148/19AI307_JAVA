# Ex.No:12(B)   COMPARABLE & COMPARATOR INTERFACE
## AIM :
To Write a java program to compare two elements , if element is greater means display 1 otherwise display -1 use only comparable interface in java collection.


## ALGORITHM :
1.	Start the Program.
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
Program to implement a COMPARABLE & COMPARATOR INTERFACE using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

public class Main implements Comparable<Main>
{
    int element;
    Main(int m)
    {
        element = m;
    }
    
    public int compareTo(Main other)
    {
        if(this.element > other.element){
            return 1;
        }
        else{
            return -1;
        }
    }
    
    public static void main(String args[])
    {
        Scanner sn = new Scanner(System.in);
        Main n1 = new Main(sn.nextInt());
        Main n2 = new Main(sn.nextInt());
        
        int res1 = n1.compareTo(n2);
        int res2 = n2.compareTo(n1);
        System.out.println(res1);
        System.out.println(res2);
        
    }
}
```






## OUTPUT:

![Screenshot 2025-05-17 181153](https://github.com/user-attachments/assets/2a958468-798d-476d-8303-a833b7678a50)



## RESULT:
Thus the java program to compare two elements , if element is greater means display 1 otherwise display -1 use only comparable interface in java collection was executed successfully




