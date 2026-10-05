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
/*
Program to implement a variable and operators using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```
class Name {
    String Fname, Mname, Lname;

    void dispName(String fn, String mn, String ln) {
        Fname = fn;
        Mname = mn;
        Lname = ln;

        System.out.println("Name: " + Fname + " " + Mname + " " + Lname);
    }
}

class Employee {
    int Emp_Id;
    Name obj = new Name();

    static String Company = "ABC Company";
    final String Country = "India";

    void disp(int id) {
        Emp_Id = id;

        System.out.println("Employee ID: " + Emp_Id);
        obj.dispName("B", "Leo", "John");
        System.out.println("Company: " + Company);
        System.out.println("Country: " + Country);
    }
}

public class Main {
    public static void main(String[] args) {
        Employee emp = new Employee();

        emp.disp(101);
    }
}

```





## OUTPUT:
<img width="558" alt="Image" src="https://github.com/user-attachments/assets/02e296c7-1a4b-4abf-87bd-cd67d25cc525" />


## RESULT:
Thus, the java program to perform final & static keyword was executed successfully.
