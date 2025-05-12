# Ex.No:4(B) INTRODUCTION TO JAVA INHERITANCE

## AIM:
To create  a Java program to perform the inheritance concept for employee details.

## ALGORITHM :
1.	Start the Program
2.	Define class `Person`:
-	a) Declare `emp_id`, `name`, and `dept` as instance variables
3.	Define class `Employee` that extends `Person`:
-	a) Define method `getDetails()`:
-	i) Create a `Scanner` object `sc`
-	ii) Read `name`, `emp_id`, and `dept` from user input
-	b) Define method `display()`:
-	i) Print the `name`, `emp_id`, and `dept`
4.	Define `Main` class with `main` method:
-	a) Create an `Employee` object `emp`
-	b) Call `getDetails()` to input employee details
-	c) Call `display()` to output employee details
5.	End








## PROGRAM:
 ```
Program to implement a Inheritance using Java
Developed by: Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java
import java.util.Scanner; 

class Person
{
    int emp_id;
    String name; String dept;
}

class Employee extends Person
{
    void getDetails()
    {
        Scanner sc = new Scanner(System.in); 
        name=sc.nextLine();
        emp_id=sc.nextInt();
        sc.nextLine(); 
        dept=sc.next();
    }
    void display()
    {
        System.out.println("Name: "+name+"Emp_ID: "+emp_id+"Department: "+dept);
    }
}

public class Main
{
    public static void main(String[] args)
    {
        Employee emp=new Employee(); 
        emp.getDetails();
        emp.display();
    }
}


```






## OUTPUT:
![alt text](<Screenshot 2025-05-12 165356.png>)


## RESULT:
Thus the Java program to implement the inheritance concept for employee details was  executed successfully.

