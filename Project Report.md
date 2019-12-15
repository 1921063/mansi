

***December 2019***

# Practical Report

## PROGROMMING FOR PROBLEM SOLVING LABORATORY                             (ESC – 105)
## Submitted By
                        NAME : MANSI
                      BRANCH :  IT
                    ROLL NO. : 1921063
         UNIVERSITY ROLL NO. : 1905362


### IT    DEPARTMENT .              GNE COLLEGE LUDHIANA


## PROGRAM 1
## Program to identify if the given number is odd or even.

#include<stdio.h>
int main()
{
int num;
printf(“type the number : \n”);
scanf(“%d”, &num);
if(num%2==0)
printf(“%d is Even.  \n”, num);
else
printf(“%d is Odd.  \n”, num);
return o;
}
## Output :
type the number :5
5 is Odd. 

## PROGRAM 2
## Program to identify if the given number is positive or negative.



#include<stdio.h>
int main()
{
double num;
printf(“enter the integer : \n”);
scanf(“%lf”, &num);
if(num<0.0)
printf(“Integer is negative.  \n”, num);
else if(num>0.0)
printf("Integer is positive.  \n”, num);
else 
printf("You entered 0.0 \n”);
return o;
}
## Output :
enter the integer :5
Integer is positive. 



## PROGRAM 3
## Program to show factorial of a given number.



#include<stdio.h>
int main()
{
int n, i, fact=1;
printf(“enter the integer : \n”);
scanf(“%d”, &n);
lf(n<0)
printf(“Factorial do not exists.  \n”);
else 
{
for(i=1;i<=n;++i)
fact *=1;
printf("Factorial of %d=%d\n”, n,fact);
}
return o;
}
## Output :
enter the integer : 5
Factorial of 5 = 125




## PROGRAM 4
## Program to show factorial of a given number using recursion.



#include<stdio.h>
long int multiplynum(int n);

int main()
{
int n;
printf(“enter the integer : \n”);
scanf(“%d”, &n);
printf("Factorial of %d=%d\n”, n,mmultiplynum(n));
return o;
}
long int multiplynum(int n)
{
if(n>=1)
return n*multiplynum(n-1);
else
return 1;
}
## Output :
enter the integer : 5
Factorial of 5 = 125



## PROGRAM 5
## Program to add two matrices.

#include <stdio.h>  
  
int main()  
{  
int m, n, c, d, first[10][10], second[10][10], sum[10][10];  
  
printf("Enter the number of rows and columns of matrix\n");  
scanf("%d%d",  &m,  &n);  
printf("Enter the elements of first matrix\n");  
  
for  (c =  0; c < m; c++)  
for  (d =  0; d < n; d++)  
scanf("%d",  &first[c][d]);  
  
printf("Enter the elements of second matrix\n");  
  
for  (c =  0; c < m; c++)  
for  (d =  0  ; d < n; d++)  
scanf("%d",  &second[c][d]);  
  
printf("Sum of entered matrices:-\n");  
  
for  (c =  0; c < m; c++)  {  
for  (d =  0  ; d < n; d++)  {  
sum[c][d]  = first[c][d]  + second[c][d];  
printf("%d\t", sum[c][d]);  
}  
printf("\n");  
}  
  
return  0;  
}
## Output :
Enter the number of rows and columns of matrix 2
2
Enter the elements of first matrix
1
2
3
4
Enter the elements of second matrix
1
2
3
4
Sum of entered matrices:-
2    4
6    8



## PROGRAM 6
## Program to check if the number is prime or not.


#include<stdio.h>
int main()
{
int n, i, flag=0;
printf(“Enter a positive integer \n”);
scanf(“%d”, &n);
for(i=2;i<n/2;++1)
{
if(n%i == 0)
{
flag=1;
break;
}
}
if(n == 1)
printf(“1 is neither prime nor composite  \n”);
else
{
if(flag == 0)
printf(“%d is a prime number.  \n”, n);
else
printf(“%d is not a prime number.  \n”, n);
}
return o;
}
## Output :
Enter a positive integer 7
7 is a prime number.
## PROGRAM 7
## Program to display multiplication table of the given number.

#include<stdio.h>
int main()
{
Int n,i;
printf(“Enter an integer:  ”);
scanf(“%d”, &n);
for(i=1;i<=10;++i)
printf(“%d * %d = %d \n”, n, i, n*i);
}
return 0;
}
## Output :
Enter an integer: 5
 5 X 1 = 5
 5 X 2 = 10
 5 X 3 = 15
 5 X 4 = 20
 5 X 5= 25
 5 X 6= 30
 5 X 7= 35
 5 X 8 = 40
 5 X 9 = 45
 5 X 10 = 50

## PROGRAM 8
## Program to display multiplication table of the given range of numbers.


#include<stdio.h>
 int main()
 {
 int x, i, t, a, b, n;
 printf(“\n \n Display table from a to b:   ”);
scanf(“%d%d”, &a , &b);
 printf(“\n \nHow many multiples should be displayed : “);
scanf(“%d”, &n);
printf(“\n \n”);
For(i=1;i<=n;i++)
{
 For(x=a;x<=b;x++)
{
t=x*1;
Printf(“%d X %d = %d \t”, x, i, t);
 }
printf(“\n”);
}
Return 0;
 }
## Output :
Display table from a to b:   3
5
How many multiples should be displayed : 2
3 X 1 = 3       4 X 1 = 4     5 X 1 = 5
3 X 2 = 6       4 X 2 = 8     5 X 2=10
# PROGRAM 9
## Program to make a simple calculator using switch case.
 #include<stdio.h>
 int main()
 {
 char operator;
double first, second;
printf(“Enter an operator (+,-,*,/):”);
scanf(“%c”, &operator );
printf(“Enter two operands: ”);
 scanf(“%lf%lf”, &first,&second );
switch(operator)
{
case’+’:
printf(“%.1lf + %.1lf = %.1lf”,  first,  second,  first+second);
break;
case’-’:
printf(“%.1lf - %.1lf = %.1lf”,  first,  second,  first-second);
break;
case’*’:
printf(“%.1lf * %.1lf = %.1lf”,  first,  second,  first*second);
break;
case’/’:
printf(“%.1lf / %.1lf = %.1lf”,  first,  second,  first/second);
break;
default:
printf(“Error! Operator is not correct”);
}
Return 0;
}
## Output :
Enter an operator (+,-,*,/): -
Enter two operands: 4
3
4.0 - 3.0 = 1.0





# PROGRAM 10
## Program to convert temperature in fahrenheit to celsius.
 #include<stdio.h>
 int main()
 {
float cel,fahr;
printf(“Enter the temp in Fahrenheit: ”);
scanf(”%f”, &fahr);
cel=(fahr-32)*5/9;
printf(“%f Fahrenheit = %f celcius \n”, fahr, cel);
Return 0;
}
## Output :
Enter the temp in Fahrenheit: 5
5.000000 Fahrenheit = -15.000000 celcius



# PROGRAM 11
## Program to find reverse of a number.
#include <stdio.h>

int  main()  
{  
int  n,  r  =  0;

printf("Enter a number to reverse\n");  
scanf("%d",  &n);

while  (n  !=  0)  
{  
r  =  r  *  10;  
r  =  r  +  n%10;  
n  =  n/10;  
}

printf("Reverse of the number = %d\n",  r);

return  0;  
}



## Output :
Enter a number to reverse
1234
reverse of the number= 4321



# PROGRAM 12
## Program to find largest in an array
#include <stdio.h>

int  main()  
{  
int  array[100],  size,  c,  location  =  0;

printf("Enter the number of elements in array\n");  
scanf("%d",  &size);

printf("Enter %d integers\n",  size);

for  (c  =  0;  c  <  size;  c++)  
scanf("%d",  &array[c]);

for  (c  =  1;  c  <  size;  c++)  
if  (array[c]  >  array[location])  
location  =  c;

printf("Maximum element is present at location %d and its value is %d.\n",  location+1,  array[location]);  
return  0;  
}

## output

Enter the size of the array: 5
 
Enter 5 elements of  the array: 12
56
34
78
100
 
largest element present in the given array is : 100

# PROGRAM 13
## Program to swap two numbers.


#include <stdio.h>

int  main()  
{  
int  x,  y,  t;

printf("Enter two integers\n");  
scanf("%d%d",  &x,  &y);

printf("Before Swapping\nFirst integer = %d\nSecond integer = %d\n",  x,  y);

t  =  x;  
x  =  y;  
y  =  t;

printf("After Swapping\nFirst integer = %d\nSecond integer = %d\n",  x,  y);

return  0;  
}


## output
Enter two integers  
23  
45  
Before Swapping  
First integer = 23  
Second integer = 45  
After Swapping  
First integer = 45  
Second integer = 23
# PROGRAM 14
## Program to display prime numbers in a given array.



  `#include  <stdio.h>`
   `int main()  {`
`int low, high, i, flag;`
 `printf("Enter two numbers(intervals): ");`
`scanf("%d %d",  &low,  &high);`
`printf("Prime numbers between %d and %d are: ", low, high);`
  `while  (low < high)  {`
    `flag =  0;`

  
  `for  (i =  2; i <= low /  2;  ++i)  {`
  `if  (low % i ==  0)  {`
  `flag =  1;`
  `break;`
  `}`
  `}`

  `if  (flag ==  0)`
  `printf("%d ", low);`
  `++low;`
  `}`

  `return  0;`
 `}`
## output
Enter two numbers(intervals): 20 
50
Prime numbers between 20 and 50 are: 23 29 31 37 41 43 47
