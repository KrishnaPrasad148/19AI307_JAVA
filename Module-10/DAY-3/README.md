# Ex.No:10(C)             JAVA LIST INTERFACE
 ## AIM :

To Create a List interface implemented by arraylist class , adding n elements to object of List interface and display the list is empty or not.


## ALGORITHM :
1.	Start
2.	Import `java.util.*`
3.	Define class `Main` with `main` method:
-	a) Initialize `Scanner` and an empty `ArrayList` named `list`
-	b) Read integer `n`
4.	Check if `list` is empty, print corresponding message
5.	Use a loop to add `n` strings to `list`
6.	Check if `list` is empty again, print corresponding message
7.	End

## PROGRAM:
 ```
Program to implement a JAVA LIST INTERFACE using Java
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
        Scanner sc=new Scanner(System.in); 
        ArrayList<String> list=new ArrayList<String>(); 
        int n=sc.nextInt();
        
        if(list.isEmpty())
        {
            System.out.println("The List is empty");
        }
        else
        {
            System.out.println("The List is not empty");
        }
        
        for(int i=0;i<n;i++)
        {
            list.add(sc.next());
        }
        if(list.isEmpty())
        {
            System.out.println("The List is empty");
        }
        else
        {
            System.out.println("The List is not empty");
        }
    }
}

```






## OUTPUT:

![Screenshot 2025-05-15 111227](https://github.com/user-attachments/assets/75dde41a-cce5-48dd-9873-239960185804)


## RESULT:
Thus the java program implemented a List interface for array list was executed and verified successfully.










