# Ex.No:8(B) IO-FILE READER/WRITER
## AIM:
To create a java program to append a String in a file “testout.txt” using Writer.


## ALGORITHM :

1. Use a `try` block to safely handle file operations.

2. Create a `FileWriter` object for the file `"testout.txt"` with `true` to enable append mode.

3. Use `write()` to add the text `"Hi Everybody"` at the end of the file.

4. Print a success message.

5. Close the `FileWriter` using `close()` to save changes.

6. If any error occurs, the `catch` block will print the exception message.

## PROGRAM:
 ```
Program to implement a IO File Reader/Writer using Java
Developed by: Krishna Prasad S
RegisterNumber: 212223230108
```

## Sourcecode.java:
```java
try
{
    FileWriter fw = new FileWriter("testout.txt", true);
    String str = "Hi Everybody";
    fw.append(str);
    fw.close();
    System.out.println("Append the character in the File Successfully");
}
catch(IOException e)
{
    System.out.println(e);
}
```

## OUTPUT:

![image](https://github.com/akshayaamanagal/19AI307_JAVA/blob/30046fcce69c38ae56989fd01721dd79977e6181/Module-08/DAY-2/image.png)

## RESULT:
Thus, the java program to append a String in a file “testout.txt” using Writer.was executed and verified successfully



