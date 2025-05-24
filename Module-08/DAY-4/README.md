# Ex.No:8(D) BUFFER INPUT/OUTPUT STREAM

## AIM:
 To create a java program file for displaying the data from the file after skip method using FileInputStream & BufferedInputStream.

## ALGORITHM :
1.	Import java.io.* and java.util.* for file handling and user input.
2.	Create a file named sample.txt and write "This is a line of text inside the file." using FileWriter.
3.	Close the FileWriter to save the content to sample.txt.
4.	Open sample.txt with a FileInputStream wrapped in a BufferedInputStream for efficient reading.
5.	Prompt the user to enter the number of bytes to skip using Scanner.
6.	Skip the specified number of bytes in the file and print the remaining content.
7.	Close the BufferedInputStream and FileInputStream to release system resources.




## PROGRAM:
 ```
Program to implement a Buffer Input/Output Stream using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

FileReader fr = new FileReader("sample.txt");
BufferedReader bfr = new BufferedReader(fr);
char[] array = new char[36];
bfr.skip(3);
bfr.read(array);
System.out.println("Data after skipping 3 characters:");
System.out.println(array);

```






## OUTPUT:

![Screenshot 2025-05-24 142008](https://github.com/user-attachments/assets/9e273086-65f1-4f7a-8439-a4960c4cfeea)


## RESULT:
Thus, the java program file for displaying the data from the file after skip method using FileInputStream & BufferedInputStream was executed and done successfully.


