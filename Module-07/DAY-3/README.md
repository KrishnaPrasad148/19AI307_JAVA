# Ex.No:7(C)             THREAD IN JAVA
## AIM:
 To Develop a Java program to create Thread using Thread class.


## ALGORITHM :
1.  Start the Program
2.	Import necessary classes: `java.util.*`
3.	Define a class `Multi` that extends `Thread`:
-	a) Create a `Scanner` instance for user input.
-	b) Override the `run` method:
-	i) Read a string from user input.
-	ii) Print "Thread Name:" followed by the input string.
4.	In the `main` method:
-	a) Create an instance of `Multi`.
-	b) Create a new `Thread` instance using the `Multi` object.
-	c) Start the thread with `t1.start()`.
5.	End





## PROGRAM:
 ```
Program to implement a Thread concepts using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

public class Multi extends Thread
{
    Scanner sc=new Scanner(System.in); 
    public void run()
    {
        String str=sc.nextLine(); 
        System.out.println("Thread Name:"+str);
    }

    public static void main(String args[])
    {
        Multi obj=new Multi(); 
        Thread t1=new Thread(obj); 
        t1.start();
    }
}

```






## OUTPUT:

![Screenshot 2025-05-14 140833](https://github.com/user-attachments/assets/9259ea8d-a85c-481d-bd75-cda8265fd3d7)


## RESULT:
Thus the Java program for the creation of Thread using Thread class was executed successfully.







