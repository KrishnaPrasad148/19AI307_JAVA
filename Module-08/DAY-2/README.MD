# Ex.No:8(B) IO-FILE READER/WRITER
## AIM:
To create a java program to append a NUMBER in a file “testout.txt” using Writer.


## ALGORITHM :
1.	It creates a file testout.txt, writes "Welcome to Java File Concept -Reader" to it, and displays this initial content.
2.	It reopens the file in append mode and adds "1234567890" at the end of the existing content.
3.	It reads the file's content (Welcome to Java File Concept -Reader1234567890) and displays it.
4.	The file is deleted using file.delete().
5.	It tries to read the file again, but this throws an exception since the file no longer exists.




## PROGRAM:
 ```
Program to implement a IO File Reader/Writer using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.io.*;

public class FileOutputStreamExample
{ 
    public static void main(String args[])
    {
        File file = new File("testout.txt"); 
        try
        {
            Writer w = new FileWriter("testout.txt");
            String content = "Welcome to Java File Concept -Reader"; 
            w.write(content);
            System.out.println("Before Appending :" +content); 
            w.close();
            
            Writer fw = new FileWriter("testout.txt",true);
            fw.append("1234567890");
            fw.close();
            System.out.println("Append the character in the File Successfull");
            FileInputStream fin=new FileInputStream("testout.txt");
            
            int i=0;
            while((i=fin.read())!=-1)
            { 
                System.out.print((char)i); 
            }
            fin.close(); 
            System.out.println(); 
            file.delete();
            
            int j=0; 
            while((j=fin.read())!=-1)
            { 
                System.out.println((char)j);
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



## RESULT:
Thus, the java program to append a NUMBER in a file “testout.txt” using Writer.was executed and verified successfully



