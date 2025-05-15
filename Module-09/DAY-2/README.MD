# Ex.No:9(B) BYTE ARRAY I/O
## AIM:
To create a java program to write data using ByteArrayOutputStream.


## ALGORITHM :
1.	The user enters a string (data), followed by two integers (start and length) specifying the starting position and number of characters to write.
2.	The string data is converted to a byte array (array).
3.	Using ByteArrayOutputStream, it writes length bytes from array, starting at start.
4.	The written data is retrieved as a string (streamData) and displayed, showing the original input and the specific segment written to the stream.
5.	Any exceptions are caught and handled, displaying stack trace information if an error occurs.




## PROGRAM:
 ```
Program to implement a BYTE ARRAY I/O using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.io.ByteArrayOutputStream;
import java.util.*;

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sn=new Scanner(System.in);
        String str = sn.nextLine();
        int start = sn.nextInt();
        int length = sn.nextInt();
        byte b[] = str.getBytes();
        
        try
        {
            ByteArrayOutputStream bar = new ByteArrayOutputStream();
            System.out.println("Original data: "+ str);
            bar.write(b, start, length);
            System.out.println("Output stream: "+ bar.toString());
            bar.close();
        }
        catch(Exception e) 
        {
            e.getStackTrace();
        }
    }
}

```






## OUTPUT:

![Screenshot 2025-05-15 104043](https://github.com/user-attachments/assets/76443dd1-6e0e-4c9e-9a41-a2d9b0b0efb8)

## RESULT:
Thus, java program to write data using ByteArrayOutputStream was executed and verified successfully.





