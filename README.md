# Amstrong-number
#include<iostream.h>
#include<conio.h>
class amstrong
{
int num,sum,t,r;
public:
void check_ams(int num)
{
t=num;
sum=0;
while( t>0 )
{
r=t%10;
sum=sum + r*r*r;
t=t/10;
}
 
if( num==sum )
cout<<"the given number is an amstrong number";
else
cout<<"the given number is not an amstrong number";
}
};
void main()
{
amstrong am;
int num;
clrscr();
cout<<"Enter the number:";
cin>>num;
am.check_ams(num);
getch();
}
