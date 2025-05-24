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

![440202870-91e15a0b-ae43-4532-9754-cce807af2c07](https://github.com/user-attachments/assets/ee8e5233-f8b7-4abc-a1d9-6e83f2e2013a)


## RESULT:
Thus, implementation of  a Java program was successfully reads a string from the user and uses StringWriter to write and print the string to the output screen.

