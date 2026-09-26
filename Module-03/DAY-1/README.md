# Ex.No:3(A)  STRING AND ITS OPERATIONS IN JAVA
## AIM:
To create a java program to read input and print length of the string in java.

## ALGORITHM :
1.  Start the Program.
2.	Import `Scanner` and define class `demo`
3.	In `main`:
-	a) Create `Scanner` object `sc`
-	b) Read a line of text into `String` variable `str`
4.	Print "The size of the String is " + `str.length()`
5.	End




## PROGRAM:
 ```
/*
Program to implement a String and its Operations using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```
import java.util.Scanner;
public class Main {
	public static void main(String[] args)
	{
    	// Here str is a string object
   	Scanner sc = new Scanner(System.in);  // Create a Scanner object
   	String str = sc.nextLine();

 
    	System.out.println(
        	"The size of "
        	+ "the String is "
        	+ str.length());
	}
}
```






## OUTPUT:

![image](https://github.com/user-attachments/assets/4182d974-4794-4220-94a1-2db096882f0b)


## RESULT:
Thus the java Program to read input and print length of the string in java was executed successfully.



# Ex.No:3(B) STRING BUFFER IN JAVA

## AIM:
To develop a java program use append() method concatenates the given argument with this String and use stringbuffer class.

## ALGORITHM :
1.	Start the program.
2.	Import `Scanner` and define class `concat`
3.	In `main`:
-	a) Create `Scanner` object `sc`
-	b) Read two strings `a` and `b` from user input
4.	Create a `StringBuffer` object `sb` initialized with string `a`
5.	Append a space and string `b` to `sb`
6.	Print the concatenated result from `sb`
7.	End







## PROGRAM:
 ```
/*
Program to implement a String Buffer using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```
import java.util.*;
public class StringBufferExample{  
public static void main(String args[]){  
Scanner sc=new Scanner(System.in);
String str1=sc.nextLine();
String str2=sc.nextLine();
StringBuffer sb=new StringBuffer(str1+" ");  
sb.append(str2);  
System.out.println(sb);  
}  
}  
```






## OUTPUT:
```
Input         Expected       Got

Hello         Hello Java     Hello Java
Java 

Hi            Hi Welcome     Hi Welcome
Welcome
```
## RESULT:
Thus the java program use append() method concatenates the given argument with this String and use stringbuffer class was executed successfully.



# Ex.No:3(C)    STRING BUILDER IN JAVA

## AIM:
To Create a java program use replace() method replaces the given String from the specified beginIndex and endIndex and use stringbuilder

## ALGORITHM :
1.  Start the Program
2.	Import `Scanner` and define class `replace`
3.	In `main`:
-	a) Create `Scanner` object `sc`
-	b) Read a string `str` from user input
4.	Create a `StringBuilder` object `sb` initialized with `str`
5.	Use the `replace()` method to replace characters from index 1 to 3 with "Java"
6.	Print the modified string using `sb.toString()`
7.	End






## PROGRAM:
 ```
/*
Program to implement a String Builder using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```
import java.util.Scanner;
public class StringBufferExample3{  
public static void main(String args[]){ 
Scanner sc=new Scanner(System.in);
String str1=sc.nextLine();
StringBuffer sb=new StringBuffer(str1);  
sb.replace(1,3,"Java");  
System.out.println(sb); 
}  
}
```




## OUTPUT:

![image](https://github.com/user-attachments/assets/236ea5c1-5152-43a3-9032-02b8ae2e1831)


## RESULT:
Thus the java program use replace() method replaces the given String from the specified beginIndex and endIndex and use stringbuilder was executed successfully.



# Ex.No:3(D) STRING TOKENIZER IN JAVA

## AIM:
To create a java program using StringTokenizer class that tokenizes a string "My name is Java Programming" on the basis of whitespace.

## ALGORITHM :
1.	Start the Program
2.	Import `Scanner` and `StringTokenizer` and define class `tok`
3.	In `main`:
-	a) Create `Scanner` object `sc`
-	b) Initialize the string `str` as "My name is Java Programming"
4.	Create a `StringTokenizer` object `token` to tokenize `str`
5.	Use a `while` loop to iterate through tokens:
-	a) Print each token using `token.nextToken()`
6.	End




## PROGRAM:
 ```
/*
Program to implement a String Tokenizer using Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:
```
import java.util.*;
public class GFG {
	public static void main(String[] args)
	{
	    Scanner sc=new Scanner(System.in);
		String str = sc.nextLine();
		String[] split = str.split(" ");
		for (int i = 0; i < split.length; i++)
			System.out.println(split[i]);
	}
}
```


## OUTPUT:

![image](https://github.com/user-attachments/assets/75834d6e-4726-4fab-a784-700c00296ddc)


## RESULT:
Thus the java program using StringTokenizer class that tokenizes a string "My name is Java Programming" on the basis of whitespace was executed successfully.



# Ex.No:3(E)  STRINGBUILDER OBJECT REFERENCE IN JAVA

## AIM:
To write a java program to calculate the number of tokens present in the tokenizer string.

## ALGORITHM :
Step 1: Start
Step 2: Import the required classes:
import java.util.* for Scanner and StringTokenizer.
Step 3: Create the Main class.
Step 4: Inside the main method:

a. Create a Scanner object to read user input.

b. Read a full line of text input from the user using nextLine().

c. Create a StringTokenizer object with the input string as its argument.

d. Use countTokens() method to count the number of tokens (words separated by whitespace by default).

e. Print the total number of tokens.

Step 5: End
## PROGRAM:
 ```
/*
Program to implement a StringBuilder Object Reference in Java
Developed by: DEEPAK K
RegisterNumber: 212224060053
*/
```

## Sourcecode.java:

```
import java.util.*;
public class Main
{
    public static void main(String[]args)
  {
        Scanner scan = new Scanner(System.in);
        String name = scan.nextLine();
        StringTokenizer st = new StringTokenizer(name);
        System.out.println("Total number of Tokens: "+st.countTokens());
   }
}

```

## OUTPUT:

![image](https://github.com/user-attachments/assets/d9e530aa-7f1f-4ce1-9845-c4a69c78b3d1)


## RESULT:
Thus the Java program successfully has calculate the number of tokens present in the tokenizer string.

