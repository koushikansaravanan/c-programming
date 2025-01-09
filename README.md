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

**ARMSTRONG NUMBERS**

#include<stdio.h>
#include<conio.h>
void main()
{
int c,x,y,a,z,b;
clrscr();
printf("***program to generate armstrong numbers***");
printf("\n armstrong numbers are ");
for(c=100;c<=999;c++)
{
x=c%100;
y=x%10;
z=c/100;
b=x/10;
a=((y*y*y)+(z*z*z)+(b*b*b));
if(c==a)
{printf("%d ",c);
}
}
getch();
}

**COMMAND LINE**

#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
void main(int argc,char*argv[])
{
  FILE *fp1,*fp2;
  char c;
  int l=0,w=0,ch=0;
  clrscr();
  if(argc!=3)
  {
   printf("invalid arguments");
   exit(0);
   }
   else
   {
    printf("copy the content of one file to anthor file \n\n");
    fp1=fopen(argv[1],"r");
    fp2=fopen(argv[2],"w");
     while((c=getc(fp1))!=EOF)
    {
    printf("%c",c);
    putc(c,fp2);
    if(c=='\n')
    l++;
    if(c==''||c=='\p'||c=='\t'||c=='\n')
    w++;
    else
    ch++;
    }
    printf("\n");
     printf("number of character :%d\n",ch);
      printf("number of words :%d\n",w);
       printf("number of lines :%d\n",l);
       fclose(fp1);
       fclose(fp2);
       }
       getch();
       }

**FIBONACCI SERIES**

#include<stdio.h>
#include<conio.h>
int fibonacci(int i)
{
if(i==0)
{
return 0;
}
if(i==1)
{
return 1;
}
return fibonacci(i-1)+fibonacci(i-2);
}
void main()
{
int i;
clrscr();
printf("the fibonacci numbers are :\n");
for(i=0;i<10;i++)
{
printf("%d\t\n",fibonacci(i));
}
getch();
}

**FILE MANIPULATION**

#include<stdio.h>
#include<conio.h>
#include<process.h>
#include<stdlib.h>
struct student
{
int rno;
char name[15];
int m1;
int m2;
}
s1;
void main()
{
int ch,n;
FILE*fp1,*fp2;
do
{
clrscr();
printf("\n 1.INSERTION");
printf("\n 2.DELETION");
printf("\n 3.MODIFICATION");
printf("\n 4.VIEW");
printf("\n 5.EXIT");
printf("\n Enter your choice:");
scanf("%d",&ch);
switch(ch)
{
case 1:
fp1=fopen("stu.txt","a");
printf("\n Enter the roll no:");
scanf("%d",&s1.rno);
printf("\n Enter the name:");
scanf("%s",s1.name);
printf("\n Enter 2 marks:");
scanf("%d%d",&s1.m1,&s1.m2);
fprintf(fp1,"\n%d\n%s\n%d\n%d",s1.rno,s1.name,s1.m1,s1.m2);
fclose(fp1);
printf("\n record inserted");
getch();
break;
case 2:
printf("\n Enter the role no to delete:");
scanf("%d",&n);
fp1=fopen("stu.txt","r");
fp2=fopen("temp.txt","w");
while(!feof(fp1))
fscanf(fp1,"\n%d\n%s\n%d\%d",&s1.rno,s1.name,&s1.m1,&s1.m2);
if(s1.rno!=n)
{
fprintf(fp2,"\n%d\n%s\n%d\n%d",s1.rno,s1.name,s1.m1,s1.m2);
}
printf("\n record deleted");
fclose(fp1);
fclose(fp2);
remove("stu.txt");
rename("temp.txt","stu.txt");
getch();
break;
case 3:
printf("\n Enter rollno to modified:");
scanf("%d",&n);
fp1=fopen("stu.txt","r");
fp2=fopen("tem.txt","w");
while(!feof(fp1))
fscanf(fp1,"\n%d\n%s\n%d\n%d",&s1.rno,s1.name,&s1.m1,&s1.m2);
if(s1.rno!=n)
{
fprintf(fp2,"\n%d\n%s\n%d\n%d",s1.rno,s1.name,s1.m1,s1.m2);
}
else
{
printf("\n old data");
printf("\n%d\n%s\n%d\n%d",s1.rno,s1.name,s1.m1,s1.m2);
printf("\n Enter the new rollno,name,mark1&mark2:");
scanf("\n%d%s%d%d",&s1.rno,s1.name,&s1.m1,&s1.m2);
fprintf(fp2,"\n%d\n%s\n%d\n%d",s1.rno,&s1.name,s1.m1,s1.m2);
}
printf("\n record updates");
fclose(fp1);
fclose(fp2);
remove("stu.txt");
rename("stemp.txt","stu.txt");
getch();
break;
case 4:
fp1=fopen("stu.txt","r");
while(!feof(fp1))
{
fscanf(fp1,"%d",&s1.rno);
printf("\n roll no=%d",s1.rno);
fscanf(fp1,"%s",s1.name);
printf("\n name=%s",s1.name);
fscanf(fp1,"%d",&s1.m1);
printf("\n mark1=%d",s1.m1);
fscanf(fp1,"%d",&s1.m2);
printf("\n mark2=%d",s1.m2);
}
fclose(fp1);
getch();
break;
case 5:
exit(0);
break;
}
}
while(ch!=5);
}

**MATRIX PROGRAM**


#include<stdio.h>
#include<conio.h>
void main()
{
int a[100][100],b[100][100],c[100][100];
int i,j,row,col,k;
clrscr();
printf("\t matrix addiation and muliplication \n");
printf("\t enter the row and column:");
scanf("%d%d",&row,&col);
printf("\t enter the first matrix :");
for(i=0;i<row;i++)
{
for(j=0;j<row;j++)
{
scanf("%d",&a[i][j]);
}
}
printf("\t enter the secound matrix");
for(i=0;i<row;i++)
{
for(j=0;j<col;j++)
{
scanf("%d",&b[i][j]);
}
}
printf("\t matrix addition:");
if(row==col)
{
for(i=0;i<row;i++)
{
for(j=0;j<col;j++)
{
c[i][j]=a[i][j]+b[i][j];
printf("\t %d",c[i][j]);
}
printf("\n\t\t\t");
}
}
else
{
printf("\n matrix addition is not possible");
}
printf("\n\t matrix multiptication:");
if(row==col)
{
for(i=0;i<row;i++)
{
for(j=0;j<col;j++)
{
c[i][j]=0;
{
for(k=0;k<row;k++)
c[i][j]=c[i][j]+a[i][j]*b[k][j];
}
printf("\t%d",c[i][j]);
}
printf("\n\t\t\t");
}
}
else
{
printf("\n matrix multiptication is not possible");
}
getch();
}

**MEDIAN PROGRAM**

#include<stdio.h>
#include<conio.h>
#include<math.h>
int main()
{
   int n,i,f[20],j,t;
   float median;
   clrscr();
   printf("\n\t\t\t program to find median");
   printf("\n enter the number of values to median:");
   scanf("%d",&n);
   printf("enter the %d values:",n);
   for(i=1;i<=n;i++)
   {
   scanf("%d",&f[i]);
   }
   for(i=1;i<=n;i++)
   {
   for(j=1;j<=n;j++)
   {
   if(f[i]<f[j])
   {
   t=f[i];
   f[i]=f[j];
   f[j]=t;
   }
   }
   }
   if(n%2==0)
   {
   median=(f[n/2]+f[n/2+1])/2.0;
   }
   else
   {
   median=f[(n/2)+1];
   }
   printf("ascending order:\n");
   for(i=1;i<=n;i++)
   {
   printf("%d \n",f[i]);
   }
   printf("median of these %d value is %f",n,median);
   return 0;
}


**NCR CALCULATION PROGRAM**

#include<stdio.h>
#include<conio.h>
int fact(int);
void main()
{
  int n,r,ncr;
  clrscr();
  printf("enter a number n:\n");
  scanf("%d",&n);
  printf("enter a number:\n");
  scanf("%d",&r);
  ncr=fact(n)/(fact(r)*fact(n-r));
  printf("value of %dc%d=%d",n,r,ncr);
  getch();
  }
  int fact(int n)
  {
  int i,f=1;
  for(i=1;i<=n;i++)
  {
  f=f*i;
  }
  return f;
  }

**N PRIME NUMBER PROGRAM**

#include<stdio.h>
#include<conio.h>
void main()
{
  int start,end,i,j,count;
  clrscr();
  printf("enter start values :");
  scanf("%d",&start);
  printf("enter end values :");
  scanf("%d",&end);
  printf("the prime numbers between %d and %d are",start,end);
  for(i=start;i<=end;i++)
  {
  count=0;
  for(j=1;j<=i;j++)
  {
  if(i%j==0)
  {
  count++;
  }
  }
  if(count==2)
  printf("%d",i);
  }
  getch();
  }

**PALINDROME PROGRAM**

#include<stdio.h>
#include<string.h>
#include<conio.h>
void main()
{
char s1[20],s2[20];
clrscr();
printf("enter a string :");
scanf("%s",&s1);
strcpy(s2,s1);
strrev(s1);
if(strcmp(s2,s1)==0)
printf("string %s is a palindrome",s1);
else
printf("string %s is not a palindrome",s2);
getch();
}

**STANDARD DEVIATION PROGRAM**

#include<stdio.h>
#include<math.h>
#include<conio.h>
void main()
{
 int n,i,f[20];
 float variance,deviation,mean,sd,sum=0.0,sumsqr;
 clrscr();
 printf("\n ***program to find standard devaition***");
 printf("\n enter the number of values:");
 scanf("%d",&n);
 printf("\nenter the %d values :",n);
 for(i=1;i<=n;i++)
 {
scanf("%d",&f[i]);
sum=sum+f[i];
}
mean=sum/(float)n;
for(i=1;i<=n;i++)
{
deviation=f[i]-mean;
sumsqr+=deviation*deviation;
}
variance=sumsqr/(float)n;
sd=sqrt(variance);
printf("\nnumber of items=%d",n);
printf("\nmean value=%f",mean);
printf("\nstandard deviation=%f",sd);
getch();
}

**STRING MANIPULATION PROGRAM**

#include<stdio.h>
#include<conio.h>
#include<string.h>
void main()
{
int 11,12,choice;
char s1[50],s2[50],ans;
clrscr();
printf"\t\t string manipulation\n");
printf("\n\t Enter two string:");
scanf("%s,%s"&s1,&s2);
do
{
printf("\n\t 1 string concentration");
printf("\n\t 2 string copy");
printf("\n\t 3 string comparision");
printf("\n\t 4 string length");
printf("\n\t 5 string reverse");
printf("\n\n\t Enter the choice");
scanf("%d",&choice);
switch(choice)
{
case 1:
strcat(s1,s2);
printf("\n\t concatenation string=%s:",s1);
break;
case 2:
strcpy(s1,s2);
printf("\n\t copied string=%s",s1);
break;
case 3:
if(strcmp(s1,s2)==0)
printf("\n\t the two strings are equal");
else
printf("\n\t the two strings are not equal");
break;
case 4:
11=strlen(s1);
printf("\n\t the length of the string is %s=",s1,l1);
12=strlen(s2);
printf("\n\t the length of the string is %s=",s2,l2);
break;
case 5:
printf("\n\t string is %s",s1);
strrev(s1);
printf("\n\t reversed string %s",s1);
printf("\n\t string is %s",s2);
break;
default:
printf("\n\t invalid choice");
}
printf("\n\n\t DO YOU WANT TO CONTINUE");
scanf("%s",&ans);
}
while (ans=='y'||ans=='N');
getch();
}

**STUDENT MARKSHEET PROGRAM**

#include<stdio.h>
#include<conio.h>
void main()
{
  struct student
  {
   char rollno[10];
   char name[20];
   int marks[5],m[10],k[10];
   }
   s[10];
   int i=0,j,n,tot=0,tot1;
   char x;
   char sub[5][10]={"tamil","english","c pro","acc","c lab"};
   char code[5][6]={"101","102","103","104","105"};
   clrscr();
   printf("\n enter the number of student:");
   scanf("%d",&n);
   for(i=1;i<=n;i++)
   {
   printf("\nroll no & name");
   scanf("%s%s",&s[i].rollno,s[i].name);
   printf("\n\tinternel marks (out of 25)");
   printf("\n\t tamil:");
   scanf("%d",&s[i].m[0]);
   printf("\n\t english:");
   scanf("%d",&s[i].m[1]);
   printf("\n\t c pro:");
   scanf("%d",&s[i].m[2]);
   printf("\n\t acc:");
    scanf("%d",&s[i].m[3]);
     printf("\n\t c lab:");
      scanf("%d",&s[i].m[4]);
      printf("\n\t external marks:(out of 75)");
   printf("\n\t tamil:");
   scanf("%d",&s[i].k[0]);
   printf("\n\t english:");
   scanf("%d",&s[i].k[1]);
   printf("\n\t c pro:");
   scanf("%d",&s[i].k[2]);
   printf("\n\t acc:");
    scanf("%d",&s[i].k[3]);
     printf("\n\t c lab:");
      scanf("%d",&s[i].k[4]);
      }
     for(i=1;i<=n;i++)
     {
      printf("\n\n\t\t\tbharathiyar university");
       printf("\n\n\tkongunadu arts and science college");
	printf("\n\t\t\t statment of mark list ");
	 printf("\n\n\t department of BCA");
	  printf("\n\t\t batch:2019-2021");
	   printf("\n\t\t name :%s",s[i].name);
	   printf("\n\nt\t name :%s",s[i].rollno);
	   printf("\n sub.code\tsubject name int.mark ext.mark totel\t result\n");
	   for(j=0;j<5;j++)
	   {
	   printf("%s",code[j]);
	   printf("\t\t%s",sub[j]);
	   printf("\t\t%d",s[i].m[j]);
	   printf("\t\t%d",s[i].k[j]);
	   tot1=(s[i].m[j]+s[i].k[j]);
	   printf("\t%d",tot1);
	   tot=tot+tot1;
	   if(s[i].k[j]>=40)
	   {
	   printf("\tpass\n");
	   }
	   else
	   {
	   printf("\tfail\n");
	   }
	   }
	   printf("\n\ttotal:%d",tot);
	   }
	   getch();
	   }


































































































