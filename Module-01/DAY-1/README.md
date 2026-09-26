# Ex.No:1(A) CLASS & OBJECTS

## AIM:
To create a class named 'Student' with String variable 'name' and String variable 'address'.

## ALGORITHM :
1.	Start the program.
2.	Define a class named 'Student'
3.	Declare a String variable 'name' and initialize it with the value "John"
4.	Declare a String variable 'address' and initialize it with the value "Chennai"
5.	Define a class named 'Test'
6.	Define the 'main' method within the 'Test' class
7.	Create an object 'obj' of the 'Student' class
8.	Print the value of 'name' and 'address' variables of the 'obj' object
9.	End



## PROGRAM:
 ```
/*
Program to implement a class & objects using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```
class Student
{
    String name;
    String address;
}
public class Main
{
    public static void main(String[] args)
   {
        Student obj= new Student();        
        obj.name="John";
        obj.address="Chennai";
        System.out.println(obj.name+" "+obj.address);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/4eeffebe-7759-467e-bf87-ccd21a978cdf)
## RESULT:
Thus, the class named 'Student' with String variable 'name' and String variable 'address' was created successfully.



# Ex.No:1(B) VARIABLES AND OPERATOR

## AIM:
To write a Java program to get values of variables 'a' and 'b' and then check if both the conditions 'a < 50' and 'a < b' are true. [Class name is ‘Demo’]

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a class named 'Demo'
4.	Implement the main method
5.	Create a new instance of the 'Scanner' class named 'sc' to read user input
6.	Read an integer 'a' from the user using the 'nextInt' method of 'sc'
7.	Read another integer 'b' from the user using the 'nextInt' method of 'sc'
8.	Check if 'a' is less than 50 or if 'a' is less than 'b'
a)	If the condition is true, print "true" using the 'print' method of 'System.out'
b)	If the condition is false, print "false" using the 'print' method of 'System.out'
9.	End

## PROGRAM:
 ```
/*
Program to implement a variable and operators using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```java
import java.util.*;
public class Demo{
    public static void main(String[] args)
    {
        Scanner input  = new Scanner(System.in);
        int a = input.nextInt();
        int b = input.nextInt();
        if(a <  50 && a <  b)
        {
            System.out.print("true");
        }
        else
        {
            System.out.print("false");
        }
    }
}
```

## OUTPUT:

```
Input    Expected   Got

23       true       true
34

124      false      false
23
```

## RESULT:
Thus, the Java program to get values of variables 'a' and 'b' and then check if both the conditions 'a < 50' and 'a < b' are true is created successfully.




# Ex.No:1(C) CONTROL STATEMENTS

## AIM:
To develop a Java program to check given number is zero or not.

## ALGORITHM :
1.	Start the program.
2.	Declare an integer variable 'num'
3.	Create a Scanner object 'sc' to read input from the user
4.	Read an integer input from the user and store it in 'num'
5.	Check if 'num' is equal to 0:
a.	If true, print "Given number is Zero"
b.	If false, print 'num' followed by " is Non-Zero"
6.	End

## PROGRAM:
 ```
/*
Program to implement a class & objects using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```
import java.util.Scanner;

public class Demo
{
    public static void main(String[] args)
    {
       Scanner sc=new Scanner(System.in);
       int num=sc.nextInt();
        if(num==0)
        System.out.println("Given number is Zero");
        else
        {
        	 System.out.println(num+ " is Non-Zero");
        }
    }
}


```

## OUTPUT:
<img width="504" alt="image" src="https://github.com/user-attachments/assets/9b9a2b38-6e99-4eba-b01f-e2e592e15150" />

## RESULT:
Thus, the Java program to check given number is zero or not was created successfully.




# Ex.No:1(D) USER DEFINED METHOD.

## AIM:
To write a Java program to calculate and print the area of a circle by defining an instance method and using local variables. The class name is Area, the method name is calculateArea(), and the return type is void.

## ALGORITHM :
1. Start the program.

2. Import the `java.util` package.

3. Define a class named `Area`.

4. Declare an instance method named `calculateArea()` with return type `void`.

5. Inside the method:
   
   a) Create a `Scanner` object to read user input.
   
   b) Declare local variables `radius` and `cirarea`.
   
   c) Read the radius value from the user.
   
   d) Calculate the area using the formula `3.14 * radius * radius`.
   
   e) Print the calculated area.

6. In the `main` method:
   
   a) Create an object of the `Area` class.
   
   b) Call the `calculateArea()` method using the object.

7. End the program.





## PROGRAM:
 ```
/*
Program to implement a User Defined Method using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```   
import java.util.*;
public class Area {
        double calculateArea()
    {
        double radius,cirarea;
        Scanner sc=new Scanner(System.in);
        radius=sc.nextDouble();
        cirarea=3.14*radius*radius;
        return cirarea;
    }
        public static void main(String[] args) {
       Area obj=new Area();
       double area=obj.calculateArea();
       System.out.println("Area of Circle is "+area);
    }
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/ed252e49-6612-47ca-b513-113432021f3c)

## RESULT:
Thus, the Java program to calculate the area of a circle using an instance method and local variables with a void return type is successfully created and executed.



# Ex.No:1(E)  STATIC VARIABLE

## AIM:
To write a Java program that determines whether a given number is odd or even using a static method. The input number is passed directly to the method, and the result is printed using simple conditional logic.

## ALGORITHM :
1. Start the program.

2. Define a class named `Main`.

3. In the `main()` method:
   a) Declare an integer variable `num` and assign it the value `7`.
   b) Call the static method `find_Oddeven(num)` and pass `num` as an argument.

4. Define a static method named `find_Oddeven(int num)`:
   a) Check if `num % 2 == 0`.
      - If true, print "`num` is even".
      - Otherwise, print "`num` is odd".

5. End the program.


## PROGRAM:
 ```
/*
Program to implement a Static Variable using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```
import java.util.Scanner;
public class Main{
public static void main (String[] args){
int num=7;
find_Oddeven(num);
}

static void find_Oddeven(int num){
  if(num%2==0) 
      System.out.println(num+" is even"); 
  else 
      System.out.println(num+" is odd");
 }
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/8f7cdb15-9d19-4cc3-8d20-2c0a25af9899)

## RESULT:
Thus, the Java program to check whether a number is odd or even using a static method with a fixed input value (7) is successfully created and executed.
