A.	Write a Java code with the class name, “acad,” and a method called “main.” Hard code the program with two integers and print the sum of those two integers.


public class acad
{
public static void main(String[] args){
int a1=5;
int a2=10;
System.out.println(a1+a2);
}
}

B. Rewrite the above code, wherein the inputs are provided by the user at
runtime and the output is printed.

import java.util.Scanner;
public class acad 
{
public static void main(String[] args){
Scanner s=new Scanner(System.in);
int a1=s.nextInt();
int a2=s.nextInt();
System.out.println(a1+a2);          }
}






















C. Write a program with the method name, “sum()” that accepts two 
      parameters from the user and print the sum of those two numbers. The 
      output format should be: 
First number is: 
Second number is: 
Sum is:	
import java.util.ArrayList;
import java.util.Scanner;


public class acad {
public static void main(String[] args){
Scanner s=new Scanner(System.in);
int p=s.nextInt();            
int q=s.nextInt();            
ArrayList<Integer> odd=new ArrayList<Integer>();
ArrayList<Integer> even=new ArrayList<Integer>();
for(int i=p;i<=q;i++){
if(i%2==0)
even.add(i);               
else
odd.add(i);                
}System.out.println("Odd numbers are:\n");
for(int i:odd)
System.out.print(i+" ");
System.out.println("\nEven numbers are:\n");
for(int i:even)
System.out.print(i+" ");
}
}















D.Write a program to accept two numbers from “stdin” and find all the odd  
     as well as even numbers present in between them. 

import java.util.ArrayList;
import java.util.Scanner;

public class acad {
public static void main(String[] args){
Scanner in=new Scanner(System.in);
int p=in.nextInt();            
int q=in.nextInt();            
ArrayList<Integer> odd=new ArrayList<Integer>();
ArrayList<Integer> even=new ArrayList<Integer>();
for(int i=p;i<=q;i++){
if(i%2==0)
even.add(i);               
else
odd.add(i);                
}System.out.println("Odd numbers are:\n");
for(int i:odd)
System.out.print(i+" ");
System.out.println("\nEven numbers are:\n");
for(int i:even)
System.out.print(i+" ");
}
}

E. Joe is scared to go to school. When her dad asked for the reason, Joe said
that she was unable to complete the task given to her by her teacher. The
task was to find the “first 10 multiples” of the number entered from
“stdin”.

import java.util.Scanner;

public class acad {
public static void main(String[] args)
{
Scanner sc=new Scanner(System.in);
int n=sc.nextInt();
System.out.println("Input: "+n);
System.out.println("O/p:");
for(int i=1;i<=10;i++){
System.out.println(n+" * "+i+" = "+(n*i));
}
}
}




F. Write a program consisting the method “sum()” and demonstrate the  
    concept of method overloading using this method. 

import java.util.Scanner;


public class acad {
public static void main(String[] args){
Scanner in=new Scanner(System.in);
int p=in.nextInt();      
int q=in.nextInt();
int r=in.nextInt();
sum(p,q);
sum(p,q,r);
}
  
public static void sum(int p,int q){
System.out.println("Sum of first 2 numbers is:"+(p+q));
}
public static void sum(int p,int q,int s){
System.out.println("Sum of all 3 numbers is:"+(p+q+s));
}
}






G.  Can you overload a method with the same return type? 
       Explain your answer with proper logic. 

The method should be overloaded with the same return type in order to
avoid ambiguity.

For example,

class A{
static int add(int a1,int a2){return a1+a2;}
static double add(int a1,int a2){return a1+a2;}
}
class B{
public static void main(String[] args){
System.out.println(Adder.add(11,11));//ambiguity
}}
In this when code is compiled it will show error as:
Overloading3.java:3: error: method add(int,int) is already defined in class A
static double add(int a1,int a2){return a1+a2;}

To overcome this problem method should be overloaded with the same return type.


H.  Write a program in Java using Arrays, that sorts the element in a  
      descending Order. 

import java.util.Arrays;
import java.util.Scanner;


public class acad {
public static void main(String[] args)
{
Scanner in=new Scanner(System.in);
int n=in.nextInt(); 
int[] arr=new int[n];
for(int i=0;i<n;i++){
arr[i]=in.nextInt();
}
Arrays.sort(arr);               
for(int i=arr.length-1;i>=0;i--){
System.out.print(arr[i]+" ");

}}}




