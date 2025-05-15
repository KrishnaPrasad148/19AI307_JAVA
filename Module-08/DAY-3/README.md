# Ex.No:8(C)             FILTER READER
## AIM:
 To create a java Program to read the content from the file by using Filter Reader 


## ALGORITHM :
1.  Start the Program
2.  Define CustomFilterReader1, extending FilterReader, and override the read() method to replace spaces with $ while reading.
2.	In main(), create a FileOutputStream and a FilterOutputStream to write "India is my country" to a file named javaFile123.txt.
3.	Write the string to the file using filter.write(), then close the FilterOutputStream.
4.	Create a FileReader to read from javaFile123.txt, and wrap it with CustomFilterReader1.
5.	Read and print each character, where spaces are replaced with $, until the end of the file.
6.	Close CustomFilterReader1 and FileReader to free resources


## PROGRAM:
 ```
Program to implement a Filter Reader using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.io.*;

class CustomFilterReader1 extends FilterReader 
{ 
    CustomFilterReader1(Reader in)
    {
        super(in);
    }
    public int read() throws IOException 
    {   
        int x = super.read();
        if ((char) x == ' ')
            return ((int) '$'); 
        else
            return x;
    }
}

public class FilterReaderExample 
{ 
    public static void main(String[] args) 
    {
        try 
        {
            FileOutputStream file1 = new FileOutputStream("javaFile123.txt"); 
            FilterOutputStream filter = new FilterOutputStream(file1);
            String s="India is my country"; 
            
            byte b[]=s.getBytes(); filter.write(b);
            Reader reader = new FileReader("javaFile123.txt"); 
            CustomFilterReader1 fr = new CustomFilterReader1(reader); 
            
            int i;
            while ((i = fr.read()) != -1) 
            { 
                System.out.print((char) i);
            }
            fr.close();
            reader.close();
        } 
        catch (Exception e) 
        { 
            e.getMessage();
        }
    }
}

```






## OUTPUT:



## RESULT:
Thus the java Program to read the content from the file by using Filter Reader  was executed and verified successfully.









