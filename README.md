# HACKER-RANK-solutions

## Day 0: Hello, World.

### Objective
In this challenge, we review some basic concepts that will get you started with this series. You will need to use the same (or similar) syntax to read input and write output in challenges throughout HackerRank. Check out the Tutorial tab for learning materials and an instructional video!

Task
To complete this challenge, you must save a line of input from stdin to a variable, print Hello, World. on a single line, and finally print the value of your variable on a second line.

You've got this!

Note: The instructions are Java-based, but we support submissions in many popular languages. You can switch languages using the drop-down menu above your editor, and the input string variable may be written differently depending on the best-practice conventions of your submission language.

Input Format

A single line of text denoting  input string (the variable whose contents must be printed).

Output Format

Print Hello, World. on the first line, and the contents of input string on the second line.

Sample Input

**Welcome to 30 Days of Code!**

Sample Output

**Hello, World. 
Welcome to 30 Days of Code!**

Explanation

On the first line, we print the string literal Hello, World.. On the second line, we print the contents of the  variable which, for this sample case, happens to be Welcome to 30 Days of Code!. If you do not print the variable's contents to stdout, you will not pass the hidden test case.

###Solution:

import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {
   public static void main(String[] args) {
      Scanner scan = new Scanner(System.in); // use the Scanner class to read from stdin
      String inputString = scan.nextLine(); // read a line of input and save it to a variable
      scan.close(); // close the scanner
      
      /*Your first line of output goes here*/
      
      System.out.println("Hello, World.");
        
      System.out.println(inputString);
   }
}
---
## Day 1: Data Types

### Objective
Today, we're discussing data types. Check out the Tutorial tab for learning materials and an instructional video!

Task
Complete the code in the editor below. The variables i, d, and s are already declared and initialized for you. You must:

1. Declare 3 variables: one of type int, one of type double, and one of type String.
2. Read 3 lines of input from stdin (according to the sequence given in the Input Format section below) and initialize your 3 variables.
3. Use the + operator to perform the following operations:
   1. Print the sum of i plus your int variable on a new line.
   2. Print the sum of d plus your double variable to a scale of one decimal place on a new line.
   3.Concatenate s with the string you read as input and print the result on a new line.
Note: If you are using a language that doesn't support using + for string concatenation (e.g.: C), you can just print one variable immediately following the other on the same line. The string provided in your editor must be printed first, immediately followed by the string you read as input.

Input Format

The first line contains an integer that you must sum with i.
The second line contains a double that you must sum with d.
The third line contains a string that you must concatenate with s.

Output Format

Print the sum of both integers on the first line, the sum of both doubles (scaled to 1 decimal place) on the second line, and then the two concatenated strings on the third line.

Sample Input

12
4.0
is the best place to learn and practice coding!
Sample Output

16
8.0
HackerRank is the best place to learn and practice coding!

Explanation

When we sum the integers 4 and 12, we get the integer 16.
When we sum the floating-point numbers 4.0 and 4.0, we get 8.0.
When we concatenate HackerRank with is the best place to learn and practice coding!, we get HackerRank is the best place to learn and practice coding!.

You will not pass this challenge if you attempt to assign the Sample Case values to your variables instead of following the instructions above and reading input from stdin.

###solution:

import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {
	
    public static void main(String[] args) {
        int i = 4;
        double d = 4.0;
        String s = "HackerRank ";
		
        Scanner scan = new Scanner(System.in);

        /* Declare second integer, double, and String variables. */
        int j;
        double e;
        String t;
        /* Read and save an integer, double, and String to your variables.*/
        j = scan.nextInt();
        e = scan.nextDouble();
        scan.nextLine();
        t = scan.nextLine();
        // Note: If you have trouble reading the entire String, please go back and review the Tutorial closely.
       //s=s.concat(t); 

        /* Print the sum of both integer variables on a new line. */
        System.out.println( i + j);
        /* Print the sum of the double variables on a new line. */
		System.out.println(d +e);
        /* Concatenate and print the String variables on a new line; 
        	the 's' variable above should be printed first. */
        System.out.println(s+t);
            
        scan.close();
    }
}

---

