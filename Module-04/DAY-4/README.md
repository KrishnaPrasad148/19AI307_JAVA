# Ex.No:4(D) FINAL & STATIC IN JAVA

## AIM:
   To create a Java program to perform final & static keyword for below situation Employee object contains member 'Emp_Id'. It contains object named name, which contains its own informations such as Fname, Mname, Lname.
 
## ALGORITHM :
1.	Start the Program.
2.	Define class `Name`:
-	a) Declare three `String` variables: `Fname`, `Mname`, and `Lname`
-	b) Define method `dispName(String fn, String mn, String ln)`:
-	i) Print the full name using the passed parameters `fn`, `mn`, and `ln`
3.	Define class `Employee`:
-	a) Declare an integer variable `Emp_Id`
-	b) Create an instance of `Name` called `obj`
-	c) Define method `disp(int id)`:
-	i) Print the employee ID
-	ii) Create a new `Name` object and call `dispName("B", "Leo", "John")` to display the name
4.	Define `Main` class with `main` method:
-	a) Create an `Employee` object `emp`
-	b) Call `emp.disp(101)` to display the employee details
5.	End






## PROGRAM:
 ```
Program to implement a final & Static using Java
Developed by: Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java
class Name
{
   String Fname; 
   String Mname; 
   String Lname;
   void dispName(String fn,String mn,String ln)
   {
      System.out.println(fn+" "+mn+" "+ln);
   }
}
class Employee
{
   int Emp_Id;
   Name obj=new Name();
   void disp(int id)
   {
      System.out.println(id); 
      Name name=new Name();
      name.dispName("B","Leo","John");
   }
}
public class Main
{
   public static void main(String[] args)
   {
      Employee emp=new Employee(); 
      emp.disp(101);
   }
}

```






## OUTPUT:
![alt text](<Screenshot 2025-05-12 174039.png>)


## RESULT:
Thus, the java program to perform final & static keyword was executed successfully.
