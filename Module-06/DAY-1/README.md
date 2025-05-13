# Ex.No:6(A)  INNER CLASS
## AIM:
To create a Java Program to implement Method Local Inner Class.

## ALGORITHM :
1.  Start the Program.
2.	Define outer class `name`:
-	a) Declare `String name` and initialize it to "Johnson"
-	b) Define inner class `inner`:
- i) Define method `display()` that prints "Name given in Outer Class is " followed by `name`
3.	In the `main` method of `name` class:
-	a) Create an instance `obj` of the `name` class
-	b) Create an instance `obj2` of the inner class `inner` using `obj`
-	c) Call `display()` on `obj2` to print the outer class name
4.	End






## PROGRAM:
 ```
Program to implement a Inner Class using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:

```java

public class Name
{
    String name="Johnson"; 

    public class inner
    {
        void display()
        {
            System.out.println("Name given in Outer Class is "+name);
        }
    }

    public static void main(String args[])
    {
        Name obj=new Name();
        name.inner obj2=obj.new inner();
        obj2.display();
    }
}

```





## OUTPUT:

![Screenshot 2025-05-13 172147](https://github.com/user-attachments/assets/2b922ae4-ca8e-47e0-8b93-c9bba3eae36a)


## RESULT:
Thus, the Java Program using Method Local Inner Class was executed successfully.

