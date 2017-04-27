# Homework20170427
#include <iostream>
#include <cmath>
using namespace std;

int main()
{
char a[100];
cout<<"请输入一个十六进制数"<<endl;
cin>>a[100];
int i=0,length;
length=strlen(a);
int ten=0;
int d[100];
for(i=0;i<=length;i++)
{d[i]= pow(16.0,i);
switch(a[i])
{
     case 0||1||2||3||4||5||6||7||8||9: ten=ten+a[i]*d[i];
	 case 'A': ten=ten+10*d[i];
	 case 'B': ten=ten+11*d[i];
	 case 'C': ten=ten+12*d[i];
	 case 'D': ten=ten+13*d[i];
	 case 'E': ten=ten+14*d[i];
	 case 'F': ten=ten+15*d[i];
	 default :{cout<<"您输入的不是十六进制数"<<endl;
		       main();}
}}
cout<<"转换成十进制数为"<<ten<<endl;
}
