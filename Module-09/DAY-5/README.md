# Ex.No:9(E) STRING WRITER

## AIM:
To write a Java program that reads a string from the user and prints it using the StringWriter class.
## ALGORITHM :

a.	Start the program.
b.	Import java.io.* and java.util.Scanner.
c.	Create a Scanner object to read input from the user.
d.	Read a string from the user.
e.	Create a StringWriter object.
f.	Write the string to the StringWriter object.
g.	Convert the StringWriter content to a string using .toString().
h.	Print the result on the output screen.
i.	Close the writer.
j.	End the program.


## PROGRAM:
 ```
Program to implement a STRING WRITER
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.io.StringWriter;
import java.util.*;

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sn = new Scanner(System.in);
        String data = sn.nextLine();
    
        try 
        {
            StringWriter sw = new StringWriter();
            sw.write(data);
            System.out.println("Data in the StringWriter: "+ sw);
            sw.close();
        }
        catch(Exception e) 
        {
            e.getStackTrace();
        }
    }
}

```






## OUTPUT:

![Screenshot 2025-05-15 105656](https://github.com/user-attachments/assets/4cf245ca-905e-4b6f-a037-a0769792bcd6)


## RESULT:
Thus, implementation of  a Java program was successfully reads a string from the user and uses StringWriter to write and print the string to the output screen.

