# Ex.No:8(A)  IO-FILE STREAM
## AIM:
To implement a Java Program to write a String in a file "testout.txt" using FileInputStream

## ALGORITHM :

1. Use `try` block to handle possible file errors.

2. Create a `FileInputStream` to read from a file named `"testout.txt"`.

3. Read one byte (character) from the file using `read()`.

4. Convert the byte to a character and print it.

5. If any error occurs (like file not found), the `catch` block runs and prints the error message.

## PROGRAM:
 ```
Program to implement a IO File Stream using Java
Developed by: Krishna Prasad S
RegisterNumber: 212223230108
```

## Sourcecode.java:
```java

try
{
   FileInputStream f=new FileInputStream("testout.txt");
   int i=f.read();
   System.out.print((char)i);
}
catch(Exception e)
{
   System.out.println(e);
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/9669903a-3242-4acf-812c-22608d76a879)



## RESULT:
Thus the implementation of a Java Program to write a String in a file "testout.txt" using FileInputStream was executed and verified successfully

