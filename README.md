# Homework20170427
#include <iostream>
#include <cmath>
using namespace std;
int main()
{
char a[100];                                                  //将数存储为字符数组
cout<<"请输入一个十六进制数"<<endl;
cin.getline(a,100);                                           
int i,length;
length=strlen(a);
int ten=0;
int d[100];
for(i=0;i<length;i++)
{d[i]= pow(16.0,length-i-1);
if(a[i]='0'||'1'||'2'||'3'||'4'||'5'||'6'||'7'||'8'||'9'||'A'||'B'||'C'||'D'||'E'||'F')
{switch(a[i])
{    case '0': ten=ten;break;
	 case '1': ten=ten+1*d[i];break;
	 case '2': ten=ten+2*d[i];break;
     case '3': ten=ten+3*d[i];break;
	 case '4': ten=ten+4*d[i];break;
	 case '5': ten=ten+5*d[i];break;
	 case '6': ten=ten+6*d[i];break;
	 case '7': ten=ten+7*d[i];break;
	 case '8': ten=ten+8*d[i];break;
	 case '9': ten=ten+9*d[i];break;
	 case 'A': ten=ten+10*d[i];break;
	 case 'B': ten=ten+11*d[i];break;
	 case 'C': ten=ten+12*d[i];break;
	 case 'D': ten=ten+13*d[i];break;
	 case 'E': ten=ten+14*d[i];break;
	 case 'F': ten=ten+15*d[i];break;}
cout<<"转换成十进制数为"<<ten<<endl;}
}}
else
cout<<"您输入的不是一个十六进制数"<<endl;

