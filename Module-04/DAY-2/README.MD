# Ex.No:4(B) INTRODUCTION TO JAVA INHERITANCE

## AIM:
To write a Java program for below situation, Student object contains member 'Stu_Id'. It contains object named course, which contains its own informations such as Degree, Branch, Year of Studying.

## ALGORITHM :

1. Start

2. Define class Subject:

   Declare four String variables: subject1, subject2, subject3, subject4.

   Create a method dispSub(String subject1, String subject2, String subject3, String subject4):

   Print the four subjects separated by spaces.

3. Define class Student:

   Declare an int variable Stu_Id.

   Create an object obj of class Subject.

   Create a method disp(int id):

   Print the student ID.

   Call dispSub method of Subject object obj, passing "B.Tech", "IT", "Third", "year".

4. Define class Main:

   In the main method:

   Create an object of Student class.

   Call the disp method on the Student object, passing 101 as the student ID.

5. End

## PROGRAM:
 ```
/*
Program to implement a Inheritance using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```

class Subject
{
    
    String subject1,subject2,subject3,subject4;
      //Write Your Code Here
      
    void dispSub(String subject1,String subject2,String subject3,String subject4)
    {
        System.out.println(subject1+" "+subject2+" "+subject3+" "+subject4);
         //Write Your Code Here
    }
}
class Student
{
    int Stu_Id;
    Subject obj = new Subject();
    
    //Write Your Code Here
    
    void disp(int id)
    {
        System.out.println(id);
        obj.dispSub("B.Tech","IT","Third","year");
        //Write Your Code Here
    }
}

public class Main
{
    public static void main(String[] args)
    {
        //Write Your Code Here
        Student obj = new Student();
        obj.disp(101);
        
    }
}
```


## OUTPUT:
```
Input      Expected                 Got
---        101                      101
           B.Tech IT Third year     B.Tech IT Third year
```
## RESULT:
Thus the Java program to implement the program for below situation, Student object contains member 'Stu_Id'. It contains object named course, which contains its own informations such as Degree, Branch, Year of Studying was  executed successfully.

