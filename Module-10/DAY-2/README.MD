# Ex.No:10(B) JAVA LINKED LIST
## AIM :
To Create a java program to perform linkedlist, read size of the list , read the elements for the linkedlist and display the elements from the linkedlist.


## ALGORITHM :
1.	Start the Program
2.	Import `java.util.*` for input handling and list functionality
3.	Define class `Hello` with the `main` method:
-	a) Create `Scanner` object `sc` for input
-	b) Read an integer `n` to specify the number of strings
-	c) Create a `LinkedList` named `str` to store strings
4.	Use a `for` loop to:
-	a) Read `n` strings from input and add each to `str`
5.	Print the entire `str` list
6.	End



## PROGRAM:
 ```
Program to implement a JAVA LINKED LIST using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

public class Hello
{
    public static void main(String args[])
    {
        Scanner sn = new Scanner(System.in);
        int n = sn.nextInt();
        sn.nextLine();
        LinkedList<String> str = new LinkedList<>();
        for(int i=0; i<n; i++)
        {
            str.add(sn.nextLine());
        }
        System.out.println(str);
    }
}

```






## OUTPUT:

![Screenshot 2025-05-15 110619](https://github.com/user-attachments/assets/e57de9fc-6d81-43b7-9661-45a30e1be52e)


## RESULT:
Thus the Java program of the creation of a linkedlist was executed successfully.





