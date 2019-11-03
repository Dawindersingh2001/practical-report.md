# **PROGRAMMING FOR PROGRAM SOLVING ESC-18105**
## NAME-*DAWINDER SINGH*
## ROLL NO-*1915019*
BRANCH-COMPUTER SCIENCE*
![LOGO](
# 1.Programs to disply a welcome message using puts
```C
#include<stdio.h>
int main()
{
puts("\nHELLO TO BUDDING ENGINEERS\n");
return 0;
}
```
Output of program
```C
HELLO TO BUDDING ENGINEERS
```
# 2. programs to disply addres using puts
```C
#include<stdio.h>
int main()
{
puts("DAWINDER SINGH \n CSE A1\n 1915019\n\VPO CHAMINDA LUDHIana"};
return 0;
``` 
output of programs 
```C
DAWINDER SINGH 
CSE A1
1915019
VPO CHAMINDA LUDHIANA
```
# 3.programs to find the sum of two number .
```C
#include <stdio.h>
int main()
{
    int firstNumber, secondNumber, sumOfTwoNumbers;
    
    printf("enter the two integer ");
    scanf("%d %d", &firstNumber, &secondNumber);
    sumOfTwoNumbers = firstNumber + secondNumber;      
    printf("%d + %d = %d", firstNumber, secondNumber, sumOfTwoNumbers);
    return 0;
}
```
Output of programs 
```C
Enter two integers: 12
11
12 + 11 = 23
```
# 4.prorams to convert Centigrate to farhnhiet .
```C
#include<stdio.h>
int main()
{
	
	float cen, fah;
	printf("Enter temperature in Celsius : ");
	scanf("%f",&cen);
	fah=(1.8 * cen) + 32;
	printf("\nTemperature in Fahrenheit = %f",fah);
	return 0;
}
```
output of programs 
```C
Enter the temerature in Celsious : 37
Temperatur in fahrenheit : 98.599998
```
# 5.programs to find the area and perimeter of circle .
```C 
#include<stdio.h>
int  main()
{

	float r, area, circum;
	printf("Enter the radius of the circle :");
	scanf("%f",&r);
	area=3.14*r*r;
	circum=2*3.14*r;
	printf("Area of the circle = %f\nCircumference of the circle = %f\n",area,circum);
	return 0;
}
```
output of programs :
```C
Enetr the radius of the circle :5
Area of the circle =78.500000
Circumference of the circle = 31.400000
```
# 6. programs to swap the two number without using third variable .
```C
#include<stdio.h>  
 int main()    
{    
int a=10, b=20;      
printf("Before swap a=%d b=%d",a,b);      
a=a+b;//a=30 (10+20)    
b=a-b;//b=10 (30-20)    
a=a-b;//a=20 (30-10)    
printf("\nAfter swap a=%d b=%d",a,b);    
return 0;  
}   
```
Output:
```C
Before swap a=10 b=20
After swap a=20 b=10
```
# 7. programs to check whether even or odd number .
```C
#include<stdio.h>
int main()
{
    int num;
    printf("Enter any number: ");
    scanf("%d", &num);
    if(num%2 == 0)
        printf("\nIt's an even number.");
    else
        printf("\nIt's an odd number.");
	
    return 0;
}
```
Output of programs 
```C
Enter any number:4
It's an even number.
```
# 8.program to find the factorial of the number .
```C
#include<stdio.h>
int main()
{
    int num, i, fact=1;
    printf("Enter any number: ");
    scanf("%d", &num);
    for(i=num; i>0; i--)
        fact = fact*i;
    printf("\nFactorial of %d = %d", num, fact);
    
    return 0;
}
```
Output the programs 
```C
Enter any number:5
factorial of 5 = 120
```
# 9. programs to fizz buzz
```C
#include <stdio.h>

int main(void)
{
    int i;
    for(i=1; i<=100; i++)
    {
        if(((i%3)||(i%5))== 0)
            printf("number= %d FizzBuzz\n", i);
        else if((i%3)==0)
            printf("number= %d Fizz\n", i);
        else if((i%5)==0)
            printf("number= %d Buzz\n", i);
        else
            printf("number= %d\n",i);

    }

    return 0;
}
```
Output the programs
```C
1
2
fizz
4
buzz
..........
```
# 10.programs to print week of days using switch case 
```C
#include <stdio.h>

int main()
{
    int week;
   
    printf("Enter week number(1-7): ");
    scanf("%d", &week);
    
    switch(week)
    {
        case 1: 
            printf("Monday");
            break;
        case 2: 
            printf("Tuesday");
            break;
        case 3: 
            printf("Wednesday");
            break;
        case 4: 
            printf("Thursday");
            break;
        case 5: 
            printf("Friday");
            break;
        case 6: 
            printf("Saturday");
            break;
        case 7: 
            printf("Sunday");
            break;
        default: 
            printf("Invalid input! Please enter week number between 1-7.");
    }

    return 0;
}
```
Output of programsg 
```C
Input week number(1-7): 2
Tuesday
```
#.11 programe to make a calculator using switch case 
```C
#include<stdio.h>
int main() {
    char operator;
    double firstNumber,secondNumber;
    printf("Enter an operator (+, -, *,): ");
    scanf("%c", &operator);
    printf("Enter two operands: ");
    scanf("%lf %lf",&firstNumber, &secondNumber);
    switch(operator)
    {
        case '+':
            printf("%.1lf + %.1lf = %.1lf",firstNumber, secondNumber, firstNumber + secondNumber);
            break;
        case '-':
            printf("%.1lf - %.1lf = %.1lf",firstNumber, secondNumber, firstNumber - secondNumber);
            break;
        case '*':
            printf("%.1lf * %.1lf = %.1lf",firstNumber, secondNumber, firstNumber * secondNumber);
            break;
        case '/':
            printf("%.1lf / %.1lf = %.1lf",firstNumber, secondNumber, firstNumber / secondNumber);
            break;
        
        default:
            printf("Error! operator is not correct");
    }
    
    return 0;
}
```
Output
```C
Enter an operator (+, -, *,): *
Enter two operands: 1.5
4.5
1.5 * 4.5 = 6.8

```
# 12. programs to cheak leap of year
```C
#include <stdio.h>
int main()
{
    int year;
    printf("Enter a year: ");
    scanf("%d",&year);
    if(year%4 == 0)
    {
        if( year%100 == 0)
        {
            
            if ( year%400 == 0)
                printf("%d is a leap year.", year);
            else
                printf("%d is not a leap year.", year);
        }
        else
            printf("%d is a leap year.", year );
    }
    else
        printf("%d is not a leap year.", year);
    
    return 0;
}
```
Output 1
```C

Enter a year: 1900
1900 is not a leap year.
```
# 13. programs to cheak prime number or not
```C
#include <stdio.h>
int main()
{
    int n, i, flag = 0;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    for(i = 2; i <= n/2; ++i)
    {
       
        if(n%i == 0)
        {
            flag = 1;
            break;
        }
    }
    if (n == 1) 
    {
      printf("1 is neither a prime nor a composite number.");
    }
    else 
    {
        if (flag == 0)
          printf("%d is a prime number.", n);
        else
          printf("%d is not a prime number.", n);
    }
    
    return 0;
}
```
Output
```C

Enter a positive integer: 29
29 is a prime number.
```
# 14. programs to find number pallindrome or not
```C
#include <stdio.h>
int main()
{
    int n, reversedInteger = 0, remainder, originalInteger;
    printf("Enter an integer: ");
    scanf("%d", &n);
    originalInteger = n;
    
    while( n!=0 )
    {
        remainder = n%10;
        reversedInteger = reversedInteger*10 + remainder;
        n /= 10;
    }
    
    if (originalInteger == reversedInteger)
        printf("%d is a palindrome.", originalInteger);
    else
        printf("%d is not a palindrome.", originalInteger);
    
    return 0;
}
```
output 
```C

Enter an integer: 1001
1001 is a palindrome.
```
