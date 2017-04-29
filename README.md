# Homework20170427
#include <iostream>
#include <cmath>
using namespace std;
int main()
{
char a[100];                                                  
cout<<"请输入一个十六进制数"<<endl;
cin.getline(a,100);                                           
int i,length;
length=strlen(a);                                            
int ten=0;                                                   
for(i=0;i<length;i++)
{   int c=a[i]; 
    int d= pow(16.0,length-i-1);
	if(c>=48&&c<=57)
      ten=ten+(c-48)*d;
	else if(c>=65&&c<=70)
      ten=ten+(c-65)*d;
	else ten=-100;}
if (-100==ten)
cout<<"您输入的不是一个十六进制数"<<endl;
else cout<<"转化为十六进制数是"<<ten<<endl;
}
