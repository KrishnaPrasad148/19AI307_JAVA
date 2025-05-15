# Ex.No:9(C)             STRING READER
## AIM:
 To Create a Java Program to display and skip the specified number of characters using the predefined Method Skip in StringReader


## ALGORITHM :
1.  The user enters a string (data) and an integer (skipnumber) indicating the number of characters to skip.
2.	The original string is displayed for reference.
3.	A StringReader object, input, is created to read from data.
4.	The program skips the specified number of characters (skipnumber) in the string.
5.	It reads and displays the remaining characters one by one until the end of the string.
6.	Any exceptions are caught, and stack trace information is generated if an error occurs.


## PROGRAM:
 ```
Program to implement a String Reader using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;
import java.io.*;

public class Main
{
    public static void main(String args[])
    {
        Scanner sn=new Scanner(System.in);
        String str = sn.nextLine();
        int n = sn.nextInt();
        System.out.println("Original data: "+ str);
        try
        {
            StringReader sr = new StringReader(str);
            sr.skip(n);
            System.out.println("Data after skipping");
            int c = sr.read();
            while(c!=-1)
            {
                System.out.print((char)c);
                c = sr.read();
            }
        }
        catch(Exception e)
        {
            System.out.println(e);
        }
    }
}

```






## OUTPUT:

![Screenshot 2025-05-15 104614](https://github.com/user-attachments/assets/d30c031a-9e91-4e26-9bf9-882938ce9147)


## RESULT:
Thus the Java Program to display and skip the specified number of characters using the predefined Method Skip in StringReader was executed and verified successfully.











