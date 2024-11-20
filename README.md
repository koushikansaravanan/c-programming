# c-programming
**ADDITION OF TWO NUMBERS**
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    printf("%d",a+b);
    
}
**INCREMENT**
#include<stdio.h>
int main()
{
    int a,b;
    a=5;
    b=a++;
    printf("%d %d",a,b);
    a=5;
    b=++a;
    printf("\n%d %d",a,b);
    a=3;
    printf("\n%d %d %d",a++,a++,a++); 
}
**ARITHEMETIC OPERATOR**
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    printf("%d %d %d %d",a+b,a-b,a*b,a/b);
}
**POSITIVE AND NEGATIVE**
#include<stdio.h>
int main()
{
    int n;
    printf("enter a number: ");
    scanf("%d",&n);
    if(n>0)
        printf("positive");
    else
       printf("negative");
}
**EVEN OR ODD**
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if(a%2==0)
    printf("even");
    else
    printf("odd");
}
**VOWEL OR CONSONANT**

#include <stdio.h>

int main()
{
    char ch;
    scanf("%c",&ch);
    if (ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u')
    printf("vowels");
    else
    printf("consonants");
}
**AREA & PERIMETER OF RECTANGULAR**
#include<stdio.h>
int main()
{
    int a,b;
    printf("Length is :");
    scanf("%d",&a);
    printf("breath is :");
    scanf("%d",&b);
    printf("area is : %d",a*b);
    printf("\nperimeter is : %d",2*(a*b));
    
}
**MAXIMUM NUMBER**
#include<stdio.h>
int main()
{
    int a,b,c;
    scanf("%d%d%d",&a,&b,&c);
    if(a>b&&a>c)
    printf("maximum number is %d",a);
    else if(b>a&&b>c)
    printf("maximum number is %d",b);
    else printf("maximum number is %d",c);
}
**MAXIMUM AND MINIMUM THREE NUMBER**
#include<stdio.h>
void main()
{
 int a,b,c;
 printf("Enter 3 numbers :");
 scanf("%d%d%d",&a,&b,&c);
 if(a>b && a>c)
  printf("Maximum number is a = %d",a);
 else if(b>a && b>c)
  printf("Maximum number is b = %d",b);
 else
   printf("Maximum number is c = %d",c);
 if(a<b && a<c)
  printf("\nMinimum number is a = %d",a);
 else if(b<a && b<c)
  printf("\nMinimum number is b = %d",b);
 else
   printf("\nMinimum number is c = %d",c);
}
**SWAP TWO NUMBERS WITHOUT USING TEMPORARY VARIABLE**
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    printf("before swapping %d %d",a,b);
    a=a+b;
    b=a-b;
    a=a-b;
    printf("\nafter swapping %d %d",a,b);
    
}

**ASK THE USER FOR THEIR NAME AND AGE AND PRINT OUT A GREETING MESSAGE**
#include <stdio.h>

int main()
{
    int age;
    char name[100];
    scanf("%d %s",&age,name);
    printf("Thanks!!");

    return 0;
}
**SUM OF DIGITS**
#include <stdio.h>

int main()
{
    int a,b,c=0;
    scanf("%d",&a);
    while(a!=0)
   {
       b=a%10;
       c+=b;
       a/=10;
   }
    printf("%d",c);

    return 0;
}
**PRINT N NATURAL NUMBER OR 10 NATURE NUMBER**
#include<stdio.h>
int main()
/*{
    int i;
    for (i=1;i<=10;i++)
    {
        printf("%d ",i);
    }
}*/ //print the first 10 natural numbers
{
    int n;
    scanf("%d",&n);
    for (int i=1;i<=n;i++)
    {
        printf("%d ",i);
    }
} //print n natural numbers
**PRINT THE MULTIPLICATION TABLE OF A GIVEN NUMBER**
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    for(int i=1;i<=b;i++)
    {
        int mul=i*a;
        printf("%d * %d = %d\n",a,i,mul);
    }
}// Print the multiplication table of a given number.

**FIND THE FACTORIAL OF A GIVEN NUMBER**
#include<stdio.h>
int main()
{
    int fact=1,n;
    scanf("%d",&n);
    for(int i=1;i<=n;i++)
    {
        fact*=i;
    }
    printf("%d",fact);    //Find the factorial of a given number
}
**CHECK A NUMBER IS PRIME NUMBER** 
#include<stdio.h>  

int main()
{
    int i, count = 0;
    int num;
    scanf("%d",&num);
    
    // checking number of divisors b/w 1 & num
    for(i = 1; i <= num; i++) {
      if(num % i == 0) 
        count += 1;
    } 
     // 0 & 1 are not prime number
       if(num == 0 || num == 1)
         printf("%d is not prime", num); 
     //if number of divisors are > 2 then not prime else prime 
       else if(count > 2) 
          printf("%d is not prime", num);
       else
         printf("%d is prime", num);

  return 0;
}

**PRIME**
#include<stdio.h>
int main()
{
    int count=0;
    int num;
    scanf("%d",&num);
    for(int i=1;i<=num;i++)
    {
        if(num%i==0)
        count+=1;
    }
    if(num==0||num==1)
    printf("%d not a prime number",num);
    else if(count>2)
    printf("%d not a prime number",num);
    else
    printf("%d is a prime number",num);
}

**PRINT THE REVERSE OF A GIVEN STRING**
#include <stdio.h>
#include <string.h>

int main() {
    char str[100];
    int len, i;

    printf("Enter a string: ");
    scanf("%s", str);

    len = strlen(str);

    printf("Reverse of the string: ");
    for (i = len - 1; i >= 0; --i) {
        printf("%c", str[i]);
    }

    return 0;
}
**BASIC CALCUATOR**
#include <stdio.h>

int main() {
    char op;
    double num1, num2, result;

    printf("Enter an operator (+, -, *, /): ");
    scanf("%c", &op);

    printf("Enter two numbers: ");
    scanf("%lf %lf", &num1, &num2);

    switch (op) {
        case '+':
            result = num1 + num2;
            break;
        case '-':
            result = num1 - num2;
            break;
        case '*':
            result = num1 * num2;
            break;
        case '/':
            // check for division by zero
            if (num2 == 0) {
                printf("Error: Division by zero.\n");
                return 1;
            }
            result = num1 / num2;
            break;
        default:
            printf("Error: Invalid operator.\n");
            return 1;
    }

    printf("%.2lf %c %.2lf = %.2lf", num1, op, num2, result);
    return 0;
}
