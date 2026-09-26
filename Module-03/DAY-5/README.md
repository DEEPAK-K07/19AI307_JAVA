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

