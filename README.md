PRINT PATTERN  1*2*3*4  5*6*7*8
For any input number N Print the following code – For below code N=4

1*2*3*4
5*6*7*8
9*10*11*12
13*14*15*16
PREREQUISITE:
Basic knowledge in Java programming, usage of loops.

ALGORITHM:
Take input from user i.e number of lines required (N value).
Take a result variable (say ‘a’) and initialize it with 1.
Take two loops one for each line (say ‘i’) and other for each digit in a particular line (say ‘j’).
Here ‘i’ loop is used to access each line from 1 to N and ‘j’ loop is used to print values in each line. For example in line 2 the value of i=2 and for contents in second line (i.e 5*6*7*8) the value for j for digit 5 is j=1 and for digit 6 is j=2.
Print ‘a’ value along with * and post increment it until the j loop reaches a value less than n.
After the j loop is finished, print the ‘a’ value without * and post increment it and go to next line.
Repeat the ‘i’ loop until it reaches ‘N’ lines.
CODE IN JAVA:
[code language=”java”]
import java.lang.*;
import java.io.*;
class Pattern
{
public static void main(String[] args)throws IOException
{
BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
int n,i,j,a=1;
System.out.print("Enter the number of Lines:");
n=Integer.parseInt(br.readLine()); /* Taking Input*/
for(i=1;i<=n;i++)
{
for(j=1;j<n;j++)
{
System.out.print((a++)+"*");
}
System.out.println(a++);
}
}
}
[/code]

TAKING INPUT:


DISPLAYING OUTPUT:


