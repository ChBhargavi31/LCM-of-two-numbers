#include<stdio.h>
int LCMcalculate(int a,int b);
int main()
{
int n1,n2,LCMof;
printf("\n recursion:find the LCM of two numbers:");
printf("input 1st number for LCM:");
scanf("%d",&n1);
printf("input 2nd number for LCM:");
scanf("%d",&n2);
if(n1>n2)
LCMof=LCMcalculate(n2,n1);
else
LCMof=LCMcalculate(n1,n2);
printf("the LCM of %d and %d:%d\n",n1,n2,LCMof);
return 0;
}
int LCMcalculate(int a,int b)
{
static int m=0;
m+=b;
if((m%a==0)&&(m%b==00))
{
return m;
}
else
{
LCMcalculate(a,b);
}
}
