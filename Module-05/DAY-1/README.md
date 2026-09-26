# Ex.No:5(A)  DATA HIDING AND ENCAPSULATION
## AIM:
To Create a java program to display the age of the person.Use access modifier private to achieve the data hiding concepts.

## ALGORITHM :
1. Start

2.  Import the Scanner class for input.

3. Define class Person:

   Declare a private int variable age.
   
   Create a method setAge(int age):
   
   Assign the input parameter age to the instance variable age.
   
   Create a method getAge():
   
   Return the value of age.

4. Define class Main:

   In the main method:
   
   Create a Scanner object scanner to read user input.
   
   Create an object p of class Person.
   
   Read an integer from the user and store it in inputAge.
   
   Call p.setAge(inputAge) to set the age in the Person object.
   
   Print "My age is " followed by the value returned by p.getAge().
   
   Close the scanner.

5. End


## PROGRAM:
 ```
/*
Program to implement a Data Hiding & Encapsulation using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```java
import java.util.Scanner;

class Person {
    private int age;

    public void setAge(int age) {
        this.age = age;
    }

    public int getAge() {
        return age;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Person p = new Person();

        int inputAge = scanner.nextInt();
        p.setAge(inputAge);

        System.out.println("My age is " + p.getAge());
        scanner.close();
    }
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/781fdc29-385a-4a25-bdb3-72d4c304f256)


## RESULT:
Thus , the  java program to display the age of the person.Use access modifier private to achieve the data hiding concepts.


# Ex.No:5(B) TIGHTLY ENCAPSULATED CLASS

## AIM:
To Create a java program to display the reverse string and  use tightly encapsulated class.
## ALGORITHM :

1. Start the program and import Scanner for user input.

2. Create a StringReverser class with:

   A private String variable text.
   
   A method setText to store user input.

   A method getReversedText that uses StringBuilder to reverse and return the text.

3. In the Main class, create:

   A Scanner object to read user input.
   
   A StringReverser object to process the input.

4. Read a string input from the user, set it using setText, and print the reversed text using getReversedText.

5. Close the Scanner and end the program.
## PROGRAM:
 ```
/*
Program to implement a tightly encapsulated class using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:


```java
import java.util.Scanner;

class StringReverser {
    private String text;

    public void setText(String text) {
        this.text = text;
    }

    public String getReversedText() {
        StringBuilder sb = new StringBuilder(text);
        return sb.reverse().toString();
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        StringReverser sr = new StringReverser();

        String input = scanner.nextLine();
        sr.setText(input);

        System.out.println(sr.getReversedText());
        scanner.close();
    }
}
```




## OUTPUT:

```
Input     Expected    Got

pot       top         top

lap       pal         pal

```

## RESULT:
Thus a java program to display the reverse string and  use tightly encapsulated classwas executed successfully.



# Ex.No:5(C)    GETTER AND SETTER METHOD

## AIM:
To Create a java program to print fibonacci series for given number , to read and display the value with the help of setter and getter method.

## ALGORITHM :
1. Start the program and import Scanner to take user input.

2. Create a Fibonacci class with:

3. A private int variable count.

   Methods setCount(int) to set the number of terms and getCount() to retrieve it.
   
   A printSeries() method to generate and print the Fibonacci series using a loop.

4. In the Main class:

   Create a Scanner object and a Fibonacci object.
   
   Read an integer input from the user to decide how many terms to generate.
   
   Set the count in the Fibonacci object and call printSeries() to display the series.

5. Close the Scanner and end the program.


## PROGRAM:
 ```
/*
Program to implement a Getter and Setter using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```java
import java.util.Scanner;

class Fibonacci {
    private int count;

    public void setCount(int count) {
        this.count = count;
    }

    public int getCount() {
        return count;
    }

    public void printSeries() {
        int n1 = 0, n2 = 1;
        for (int i = 0; i < count; i++) {
            System.out.print(n1 + " ");
            int next = n1 + n2;
            n1 = n2;
            n2 = next;
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Fibonacci fib = new Fibonacci();

        int input = sc.nextInt();
        fib.setCount(input);
        fib.printSeries();

        sc.close();
    }
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/3f2c59a9-3be2-4162-af36-f7a26eb2f318)


## RESULT:
Thus the java program to print fibonacci series for given number , to read and display the value with the help of setter and getter method.was executed successfully.





# Ex.No:5(D) IS-A RELATIONSHIP AND HAS-A RELATIONSHIP
## AIM:
   To Create a java program create a three class and apply is-a relationship concepts and display the output refer sample test.
 
## ALGORITHM :

1. Start the program.

2. Create a class Animal with a method eat() that prints "I can eat".

3. Create a class Person that inherits from Animal, and add a method name() that prints "My name is Rohu".

4. Create a Main class that inherits from Person:

   In the main method:
      
      Create an object of Main.
      
      Call name() to print the name.
      
      Call eat() to print the eating ability.

5. End the program.

## PROGRAM:
 ```
/*
Program to implement a IS-A RELATIONSHIP AND HAS-A RELATIONSHIP using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```java
class Animal {
    public void eat() {
        System.out.println("I can eat");
    }
}

class Person extends Animal {
    public void name() {
        System.out.println("My name is Rohu");
    }
}

public class Main extends Person {
    public static void main(String[] args) {
        Main obj = new Main();
        obj.name();
        obj.eat();
    }
}
```


## OUTPUT:

![image](https://github.com/user-attachments/assets/1846d70a-097b-4b4d-a830-f0f1da459732)


## RESULT:
Thus the java program to find factorial of number using class and object concepts and apply the has-a relationship was executed successfully.



# Ex.No:5(E) HAS-A RELATIONSHIP
## AIM:
To implement a java program for area of triangle with the help of getter and setter method and to print the value of area of triangle.
## ALGORITHM :

1. Start the program and import Scanner for user input.

2. Create a TriangleArea class with:

   Private variables width and height.
   
   Methods setWidth(double) and setHeight(double) to assign values.
   
   Method getArea() that returns the area by multiplying width and height.

3. In the main method:

   Create a Scanner object and a TriangleArea object.
   
   Read two double inputs from the user (for width and height).

4. Set the width and height in the TriangleArea object and calculate the area.

5. Print the area (after converting it to an integer) and close the scanner.
## PROGRAM:
 ```
/*
Program to implement a HAS-A RelationShip
Developed by: DEEPAK K
RegisterNumber: 212224060053 
*/
```

## Sourcecode.java:


```java
import java.util.Scanner;
public class TriangleArea {

    private double width;
    private double height;

    public void setWidth(double width) {
        this.width = width;
    }

    public void setHeight(double height) {
        this.height = height;
    }

    public double getArea() {
        return width * height;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TriangleArea triangle = new TriangleArea();
        double w = sc.nextDouble(); 
        double h = sc.nextDouble(); 
        triangle.setWidth(w);
        triangle.setHeight(h);
        System.out.println((int)triangle.getArea());
    }
}

```

## OUTPUT:

![image](https://github.com/user-attachments/assets/6761079b-9734-42e3-bbcd-705e07963810)


## RESULT:
Thus the java program to Find the Largest or Max Number in Array using has - a relationship was executed successfully. 

