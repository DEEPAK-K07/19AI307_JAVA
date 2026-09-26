# Ex.No:4(A)  JAVA CONSTRUCTOR
## AIM:
To create a Java program using constructor to print the circumference of rectangle.[l=5,w=6]

## ALGORITHM :
1.  1.	Start the Program.
2.	Define a class `circum`
3.	Inside the class, define two integer variables `l` and `w` with values 5 and 6, respectively
4.	Create a constructor `circum()`:
-	a) Calculate the `circumference` as `2 * (l + w)`
-	b) Print the `circumference` twice with different labels ("Area of First Rectangle" and "Area of Second Rectangle")
5.	In `main`, create an object `sc` of the `circum` class
6.	End





## PROGRAM:
 ```
/*
Program to implement a Constructor using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```
class Rectangle 
{ 
    int l; 
    int b; 
    
    Rectangle(int l, int b) 
    {  
        this.l = 5;
        this.b = 6;
    } 
    
    Rectangle(Rectangle obj) 
    {
        this.l = obj.l;
        this.b = obj.b;
    } 
    
    int circumference() 
    { 
        return 2*(this.l + this.b)+8;
    } 
 } 
class prog 
{ 
    public static void main(String[] args) 
    { 
        Rectangle firstRect = new Rectangle(5,6); 
        Rectangle secondRect = new Rectangle(firstRect); 
        
        System.out.println("Area  of First Rectangle : "+firstRect.circumference());
        System.out.print("Area of First Second Rectangle : "+secondRect.circumference());
     
    } 
} 
 
```



## OUTPUT:

![image](https://github.com/user-attachments/assets/eb21e576-3b9f-4a7a-b50a-fa4656dfb960)


## RESULT:
Thus the Java program using constructor to print the circumference of rectangle was executed successfully.

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
Developed by: Keerthivasan K S
RegisterNumber: 212224230120
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

# Ex.No:4(C)    CONSTRUCTOR CHAINING(SUPER KEYWORD)

## AIM:
To Create a class named 'Gadgets' which includes methods display(). [display() will print "I am a Gadget"]

Create a child class of 'Gadgets' named 'Laptop' and add a new overriding method named display() [display() will print "I am a Laptop"]  and print(). [ print() calls both overriding and overridden methods]

Create a instance of Laptop class and invoke the print method using object.

## ALGORITHM :

Step 1: Start

Step 2: Define a class Gadgets

a. Create a method display()

b. Inside display(), print "I am a Gadget"

Step 3: Define a class Parrot that extends Gadgets

a. Override the display() method

b. Inside the overridden display(), print "I am a Laptop"

c. Create a new method print()

d. Inside print(), use super.display() to call the parent class (Gadgets) version of display()

Step 4: Define the Main class with main() method

a. Create an object obj of class Parrot

b. Call obj.display() → Executes Parrot class's display() method

c. Call obj.print() → Executes Parrot class's print() method, which in turn calls Gadgets class's display() method using super

Step 5: End



## PROGRAM:
 ```
/*
Program to implement a Constructor Chaining using Java
Developed by: Keerthivasan K S
RegisterNumber: 212224230120
*/
```

## Sourcecode.java:

```

class Gadgets {

  //Write Your code Here
  void display()
  {
      System.out.println("I am a Gadget");
  }
}

class Parrot extends Gadgets {

//Write Your code Here  
void display()
{
    System.out.println("I am a Laptop");
}
void print()
{
    super.display();
}
  
}

public class Main {
  public static void main(String[] args) {
      
      //Write Your code Here
      Parrot obj=new Parrot();
      obj.display();
      obj.print();
  }
}

```





## OUTPUT:

![image](https://github.com/user-attachments/assets/240c300f-e074-4f6e-ba85-ca586e2ca81c)


## RESULT:
Thus the java program to To Create a class named 'Gadgets' which includes methods display(). [display() will print "I am a Gadget"] Create a child class of 'Gadgets' named 'Laptop' and add a new overriding method named display() [display() will print "I am a Laptop"]  and print(). [ print() calls both overriding and overridden methods] Create a instance of Laptop class and invoke the print method using object. was executed successfully.




# Ex.No:4(D) FINAL & STATIC IN JAVA

## AIM:
   To create a Java program for below situation, Student object contains member 'Stu_Id'. It contains  object named subject, which contains its own informations such as subject1,subject2,subject3,subject4.
 
## ALGORITHM :
1. Start

2. Define class Subject:

   Declare four String variables: subject1, subject2, subject3, subject4.
   
   Define method dispSub(String s1, String s2, String s3, String s4):
   
   Assign s1 to subject1.
   
   Assign s2 to subject2.
   
   Assign s3 to subject3.
   
   Assign s4 to subject4.
   
   Print the four subject names together with spaces between them.

3. Define class Student:

   Declare an int variable Stu_Id.
   
   Create an object sub of the Subject class.
   
   Define method disp(int id, String s1, String s2, String s3, String s4):
   
   Assign id to Stu_Id.
   
   Print Stu_Id.
   
   Call dispSub method of sub object, passing the four subject names s1, s2, s3, and s4.

   Define class Main:

4. In the main method:

   Create an object st of Student class.
   
   Call the disp method on st, passing:
   
   Student ID: 101
   
   Subjects: "Java", "DS", "TOC", "CG"

5. End






## PROGRAM:
 ```
/*
Program to implement a final & Static using Java
Developed by: Keerthivasan K S
RegisterNumber: 212224230120
*/
```

## Sourcecode.java:
```
class Subject {
    String subject1, subject2, subject3, subject4;

    void dispSub(String s1, String s2, String s3, String s4) {
        subject1 = s1;
        subject2 = s2;
        subject3 = s3;
        subject4 = s4;
        System.out.println(subject1 + " " + subject2 + " " + subject3 + " " + subject4);
    }
}

class Student {
    int Stu_Id;
    Subject sub = new Subject();

    void disp(int id, String s1, String s2, String s3, String s4) {
        Stu_Id = id;
        System.out.println(Stu_Id);
        sub.dispSub(s1, s2, s3, s4);
    }
}

public class Main {
    public static void main(String[] args) {
        Student st = new Student();
        st.disp(101, "Java", "DS", "TOC", "CG");
    }
}
```






## OUTPUT:

![image](https://github.com/user-attachments/assets/70c0a76a-f3e3-49f4-9590-84e1f38706ef)


## RESULT:
Thus, the java program for below situation, Student object contains member 'Stu_Id'. It contains  object named subject, which contains its own informations such as subject1,subject2,subject3,subject was executed successfully.
# Ex.No:4(E)  PARAMETERIZED CONSTRUCTOR
## AIM:
To write a parameterized constructor in the Laptop class given below that initializes the brand , price class field with the string "Apple" and 42500.75.

Call the getBrand() method in the main method of the Sample class  and store the value of the brand in a variable, and print the value.

Call the getPrice() method in the main method of the Sample class  and store the value of the price in a variable, and print the value.

## ALGORITHM :

1. Start

2. Define class Laptop:

    Declare a String variable brand.
    
    Declare a double variable price.
    
    Create a constructor Laptop():
    
    Set brand to "Apple".
    
    Set price to 42500.75.

3. Define a method getBrand():

    Return the value of brand.
    
    Define a method getPrice():
    
    Return the value of price.

4. Define class Sample:

    In the main method:
    
        Create an object myLaptop of class Laptop.
        
        Call getBrand() method using myLaptop and store the result in laptopBrand.
        
        Print laptopBrand.
        
        Call getPrice() method using myLaptop and store the result in laptopPrice.
        
        Print laptopPrice.

5. End


## PROGRAM:
 ```
/*
Program to implement a Parameterized Constructor Using Java
Developed by: Keerthivasan K S
RegisterNumber: 212224230120 
*/
```

## Sourcecode.java:

```
class Laptop {
    String brand;
    double price;
    public Laptop() {
        this.brand = "Apple";
        this.price = 42500.75;
    }

    public String getBrand() {
        return brand;
    }

    public double getPrice() {
        return price;
    }
}
public class Sample {
    public static void main(String[] args) {
        Laptop myLaptop = new Laptop();
        String laptopBrand = myLaptop.getBrand();
        System.out.println(laptopBrand);
        double laptopPrice = myLaptop.getPrice();
        System.out.println(laptopPrice);
    }
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/dd258499-d8e9-427a-97a0-9157d4055a30)


## RESULT:
Thus, the  java program was successfully parameterized constructor in the Laptop class given below that initializes the brand , price class field with the string "Apple" and 42500.75.

 



