# strong-number-between-any-two-numbers.
#include<stdio.h>
int main()
{  
    int i,n,b,sum,a,digit,prod;
    for(n=2;n<=1000000;n++)
    {
    b=a=n;
    sum=0;
    while(b>0)
       {
           digit=b%10;
           b=b/10;
           prod=1;
           for(i=1;i<=digit;i++)
           prod=prod*i;
           sum=sum+prod;
        }
if(sum==a)
printf("%d is STRONG:\n",a);
}
return 0;
}
