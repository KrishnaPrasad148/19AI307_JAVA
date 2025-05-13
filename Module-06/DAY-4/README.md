# Ex.No:6(D) PACKAGES
## AIM:
  To create a Java Program for accessing package from another package using packagename.
 
## ALGORITHM :
1.	Start the Program
2.	Create a directory named pack and save A.java inside it.
2.	Compile A.java from the parent directory using javac pack/A.java.
3.	Create another directory named mypack and save B.java inside it.
4.	Compile B.java from the parent directory using javac mypack/B.java.
5.	Run B from the parent directory with java mypack.B


## PROGRAM:
 ```
Program to implement a Packages using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

//save by A.java
package pack; 
public class A
{
    public void msg()
    {
        System.out.println("Hello");
    }
}

//save by B.java 
package mypack;
import pack.*;
class B
{
    public static void main(String args[])
    { 
        A obj = new A();
        obj.msg();
    }
}

```






## OUTPUT:

![Screenshot 2025-05-13 181046](https://github.com/user-attachments/assets/f6cded76-e461-497b-845f-aa2e696c39cd)


## RESULT:
Thus, the program has accessed the package from another package has been done successfully.

