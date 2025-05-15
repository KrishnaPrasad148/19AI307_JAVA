# Ex.No:9(A)          DATA I/O STREAM
## AIM:
To create a Java Program to store a String Value in a file "testout.txt" using Data Output Stream.

## ALGORITHM :
1.  The program creates testout.txt and initializes FileOutputStream and DataOutputStream. It prompts the user to enter a string, writes it to testout.txt using writeUTF(), and then closes the streams.
2.	It reopens testout.txt with FileInputStream and DataInputStream, reads the stored string using readUTF(), displays it, and then closes the streams.
3.	It deletes testout.txt.
4.	After deletion, it tries to read an integer from testout.txt, which causes an error because the file no longer exists.
5.	The program catches and displays an IOException message if any file-related error occurs, including the attempt to read after deletion.


## PROGRAM:
 ```
Program to implement a DATA I/O STREAM using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.io.*;
import java.util.*;

public class FileOutputStreamExample
{
    public static void main(String args[]) throws IOException
    {
        File file = new File("testout.txt");
        try
        {
            FileOutputStream fout=new FileOutputStream("testout.txt"); 
            DataOutputStream dout=new DataOutputStream(fout);
            
            Scanner sc=new Scanner(System.in); 
            String str=sc.nextLine(); 
            dout.writeUTF(str);
            dout.close();
            fout.close();
            System.out.println("Successfully Completed"); 
            
            FileInputStream fin=new FileInputStream("testout.txt"); 
            DataInputStream di=new DataInputStream(fin); 
            
            System.out.println("String: " + di.readUTF());
            fin.close();
            di.close();
            file.delete();
            int b=di.readInt();
        }
        catch(IOException e)
        {
            System.out.println("File Closed:"+e);
        }
    }
}

```






## OUTPUT:



## RESULT:
Thus the Java Program to store a String Value in a file "testout.txt" using DataOutputStream was executed and verified successfully.

