# ProblemSolving

My Youtube channel link :
https://www.youtube.com/@SunilTech218
class 2:


input n 
you need to check wheather it is even or odd
=====================
if input will be some marks 
output will be the grade

input 95 - A
 for A grade its in between 90 to 100

input 85 -B
 for B grade its in between 80 to 100

59 and below it should be fail
=================================

if there is no loop it is O(1)
---------------------------------
if there a single loop it is O(n)

for(){
}
---------------------------------
if there is a nested loop O(n^2)
for(){
  for(){
  }
}
----------------------------------
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        Scanner sc=new Scanner(System.in);
        System.out.println("Please enter the marks");
        int marks=sc.nextInt();
        
        if(marks>=90 && marks<=100){
            System.out.println("A grade");
        }else if(marks>=80 && marks<90){
            System.out.println("B grade");
        }else if(marks>=70 && marks<80){
            System.out.println("C grade");
        }else if(marks>=60 && marks<70){
            System.out.println("D grade");
        }else{
            System.out.println("Fail ");
        }
        
        //Time complexity
        //if any loop 0(n)
        //if there is no loop is involved it is 0(1);
        
        //if else if
        
        
    }
}====================================

for loop 

for(int i=0;i<n;i++)
{
  statements;
}
====================================
one is initialization will be executed only once per loo[p
condition check
statements execution
increment/decrement
========================================
program 3:
==========
if inpout 100

1 2 3 4.............100
=================================

for(int i=1;i<=100;i++)
{
  System.out.println(i);
}
==================================
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        Scanner sc=new Scanner(System.in);
        System.out.println("Please enter the value of n");
        int n=sc.nextInt();
        
        for(int i=1;i<=n;i++){
            if(i%2==1)
            System.out.print(i+" ");
        }
        
       
        
        //Time complexity
        //if any loop 0(n)
        //if there is no loop is involved it is 0(1);
        
        //if else if
        
        
    }
}
=======================================
p4:
if the input is n
output: sum of n natural numbers
=======================================
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        Scanner sc=new Scanner(System.in);
        System.out.println("Please enter the value of n");
        int n=sc.nextInt();
        int sum=0;
        for(int i=1;i<=n;i++){
            if(i%2==1)
            sum=sum+i;
        }
        //first right side part will be executed
        //and it is assigned to left
        //sum=0+1=1
        //sum=1+2=3
        //sum=3+3=6
        
        
       System.out.println(sum);
        
        //Time complexity
        //if any loop 0(n)
        //if there is no loop is involved it is 0(1);
        
        //if else if
        
        
    }
}
==================================================================
P5 
if the input is some number = n

you need to check wheather the number is prime or not

Amazon sde1 - Optimization
=============================================================

n=23

you need to divide 1 to 23

with n


23%1==

23%2==

23%3==
...............

where ever you are getting remainder as 0
that number itself is a factor

if my count=2 ie prime else not
==============================================
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        Scanner sc=new Scanner(System.in);
        System.out.println("Please enter the value of n");
        int n=sc.nextInt();
       int count=0;
       for(int i=1;i<=n;i++){
           if(n%i==0)
           count++;
       }
       if(count==2){
           System.out.println("Number is Prime");
       }else{
           System.out.println("Number is not prime");
       }
        
    }
}
===========================================
1 crore then you need 1 crore iterations

2 to n/2

if there is atleast one factor between 2 to n/2 you can break loop print not prime
50 lakhs

50 laks is also a big number
=============================================================
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        Scanner sc=new Scanner(System.in);
        System.out.println("Please enter the value of n");
        int n=sc.nextInt();
       int count=0;
       int sqr=(int)Math.sqrt(n);
       for(int i=2;i<=sqr;i++){
           if(n%i==0)
          {
              count++;
              break;
          }
       }
       if(count==1){
           System.out.println("Number is not Prime");
       }else{
           System.out.println("Number is  prime");
       }
        
    }
}

10000= 10^4= 100

1000000 = 1000

100000000= 10000

Binary Search :

=================================================================

if you really like my Teaching interested to learn DSA

Online 250 programs on Hackerank , leetcode , GFG ,Coding ninjas

You can Target some top product based companies

7pm 

8k 
10k with recordings (1 year validity)
===========================================================

Armstrong number :

153 = 1+125+27 =153

you need to check whether the number is Armstrong or not
==============================================================


153%10 = 3   153/10 = 15

get the last digit
cube it
add to sum
remove last number
==================================










Class 3 :

prog 1:
========

*****
*****
*****
*****
*****

if n=5 5X5 grid
if n=10 10X10 grid


for(i=0;i<n;i++)
{
  for(j=0;j<n;j++)
  {
  }
}



i=0 => j=0 to n-1

i=1 => j=0 to n-1



*****
***

import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        Scanner scan=new Scanner(System.in);
        int n=scan.nextInt();
        
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                System.out.print("*");
            }
            System.out.println();
        }
        //i=0 j=0 to 4
        //i=1 j=0 to 4
    }
}
=============================
program 2:
================
$****
*$*** //i=1 and j=1
**$** //i=2 and j=2
***$*
****$

=======================
program 3
===========
$***$  i=0 and j=4 => i+j=n-1
*$*$*  i=1 and j=3 => i+j=n-1
**$**
*$*$*
$***$
========================

in evening DSA class at 7pm 
===========================
program 4:
=========
*
**
***
****
*****
=======================

I iter in first row

2 iter in second row

you need to go for variable iterations in inside loop

for(i=0;i<n;i++)
{
   for(j=0;j<=I;j++)
  {
  }
}

i=0 => j=0
i=1 => j=0 ,1
i=2 => j=0,1,2
i=3 => j=0,1,2,3
i=4 => j=0,1,2,3,4
=======================









