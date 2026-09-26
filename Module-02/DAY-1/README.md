# Ex.No:2(A)  STATIC METHOD

## AIM:
To create a java program for calculate cube of a number using static method.

## ALGORITHM :
1.  Start : Begin the process of calculating the cube of a number.
2.	Declare a variable to store input : Declare an integer variable n to hold the number whose cube will be calculated.
3.	Create a Scanner object : Create a Scanner object (sc) to read the input from the user.
4.	Read input from the user : Prompt the user to input an integer value. The input value is stored in the variable n.
5.	Call the cubecal function : Call the function cubecal(n) which computes the cube of the number by performing n * n * n.
6.	Store the result : Store the result of the cubecal function in an integer variable result.
7.	Output the result :
8.	Print the cube of the number using System.out.println("Cube is: " + result);.
9.	End the program.




## PROGRAM:
 ```
/*
Program to implement a Static method using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053

*/
```

## Sourcecode.java:

```
import java.util.Scanner;

public class CubeCalculator {

    public static int calculateCube(int number) {
        return number * number * number;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int inputNumber = scanner.nextInt();
        int cube = calculateCube(inputNumber);
        System.out.println("Cube is: " + cube);

        scanner.close();
    }
}

```







## OUTPUT:


<img width="386" alt="image" src="https://github.com/user-attachments/assets/4756def7-b7e2-42ec-acf4-fde55b23fcf0" />



## RESULT:
Thus the java program for calculate cube of a number using static method has been executed successfully.



# Ex.No:2(B) ACCESS MODIFIERS

## AIM:
To develop a Java Program to display the addition number using private modifiers only.

## ALGORITHM :
1.	Start the program.
2.	Define a class named `addition`
3.	Declare two private integer variables, `num1` and `num2`
4.	Define a private method `add()` that:
a)	Returns the sum of `num1` and `num2`
5.	Define a public method `display(int n1, int n2)` that:
a)	Assigns `n1` to `num1` and `n2` to `num2`
b)	Calls the `add()` method and prints the result using `System.out.println`
6.	Define the `main` method as static
a)	Create an instance of the `addition` class called `ad`
b)	Call the `display(8, 9)` method on the `ad` object
7.	End






## PROGRAM:
 ```
/*
Program to implement a access modifiers using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```
public class A
{ 
    private void display() 
    { 
        int a=8,b=9;
        System.out.println(a+b); 
    }
    public static void main(String args[])
    {
        A obj= new A();
        obj.display();
    }
}

```






## OUTPUT:

```
Expected    Got 

17          17
```

## RESULT:
Thus the java program to display the addition number using private modifiers only was executed successfully.



# Ex.No:2(C)    SINGLE ARRAY

## AIM:
To create a java program to read 5 values and display the all 5 values from array using single dimensional array.

## ALGORITHM :
1.	Start the program.
2.	2.	Import the `Scanner` class from the `java.util` package
3.	Define a class named `ArrayExample`
4.	Inside the `main` method:
-	a) Create a `Scanner` object called `scanner` to take user input
-	b) Declare an integer array `values` of size 5
-	c) Use a `for` loop to iterate from `i = 0` to `i < 5`:
-   d) Take input from the user and store it in `values[i]`
5.	Print "Elements in Array are :"
6.	Use another `for` loop to iterate from `i = 0` to `i < 5`:
-	a) Print each element in `values` followed by a space
7.	Close the `scanner` to release resources
8.	End





## PROGRAM:
 ```
/*
Program to implement a Single Array using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```

import java.util.*;

public class Main
{
   public static void main(String args[])
   {    

	Scanner sc=new Scanner(System.in);
	
	int a[]=new int[5];//declaration    	 
	
        for(int i=0; i<5; i++)
        {
           a[i] = sc.nextInt();
        }   
        System.out.print("Elements in Array are :\n");
        for(int i=0; i<5; i++)
        {
           System.out.print(a[i] + "  ");
        }  
   }
}
	


```






## OUTPUT:
```
Input       Expected                                  Got

3           Elements in Array are :                   Elements in Array are :                   
            3  4  5  6  7                             3  4  5  6  7
4
5
6
7


```


## RESULT:
Thus, the Java program Thus the java program to read 5 values and display the all 5 values from array using single dimensional  was executed successfully.



# Ex.No:2(D) MULTI-DIMENSIONAL ARRAY

## AIM:
To create a java program that returns the sum of all the values in a 2D array.

## ALGORITHM :
1.	Start the program.
2.	Import `Scanner` and define class `sum`
3.	In `main`:
-	a) Create `Scanner` object `sc`
-	b) Read `rows` and `cols` from user
-	c) Declare 2D array `arr[rows][cols]`
4.	Populate `arr` using nested loops with user input
5.	Initialize `sum` to `0`
6.	Calculate the sum of all elements in `arr` using nested loops
7.	Print "The sum of all values in the 2D array is: " + `sum`
8.	End



## PROGRAM:
 ```
/*
Program to implement a Multi Dimensional Array using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```
import java.util.Scanner;

public class LargestElement {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int size = scanner.nextInt();
        int[] array = new int[size];

        for (int i = 0; i < size; i++) {
            array[i] = scanner.nextInt();
        }

        int largest = array[0]; // Assume the first element is the largest initially

        for (int i = 1; i < size; i++) {
            if (array[i] > largest) {
                largest = array[i];
            }
        }

        System.out.println("The largest element in the array is: " + largest);

        scanner.close();
    }
}

```







## OUTPUT:

<img width="761" alt="image" src="https://github.com/user-attachments/assets/815af82b-dc82-46f2-b13f-96ce82432fbd" />



## RESULT:
Thus the java program that returns the sum of all the values in a 2D array was executed successfully.




# Ex.No:2(E)  SMALLEST ELEMENT IN AN ARRAY

## AIM:
To write a Java program that reads an array size and elements from the user and then finds and prints the smallest element in the array.
## ALGORITHM :
1.	Start the program.
2.	Read the size of the array from the user.
3.	Declare an array of the given size.
4.	Read the array elements from the user.
5.	Initialize a variable min with the first element of the array.
6.	Traverse the array using a loop.
7.	Compare each element with min. If an element is smaller, update min.
8.	After the loop ends, print the smallest number.
9.	End the program.
	

## PROGRAM:
 ```
/*
Program to implement a Smallest Element in an Array
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```
import java.util.Scanner;

public class LargestElement {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int size = scanner.nextInt();
        int[] array = new int[size];

        for (int i = 0; i < size; i++) {
            array[i] = scanner.nextInt();
        }

        int largest = array[0]; // Assume the first element is the largest initially

        for (int i = 1; i < size; i++) {
            if (array[i] > largest) {
                largest = array[i];
            }
        }

        System.out.println("The largest element in the array is: " + largest);

        scanner.close();
    }
}

```





## OUTPUT:

<img width="759" alt="image" src="https://github.com/user-attachments/assets/7bb0f0a3-f60f-4e0a-ab84-8e9e3d8bc429" />



## RESULT:
Thus the java program successfully reads the array size and elements from the user and correctly finds and prints the smallest number in the array.



