# schoolwork-code
#include "stdafx.h"
#include "iostream"
using namespace std;

int main( )
{
	int n,i,a,b;
	
	cout<<"Please enter the number of triangle rows you want:";
	
    std::cin >>n;

	for( i=1;i<=n;i++)/*控制行数*/
		{	
			
			for(  a=n-1;a>=i;a--)//打印空格
				cout<<" ";
			   
			for(  b=1;b<=2*i-1;b++)//打印*
				cout<<"*";
			cout<<"\n";
			}
		cout<<endl;//没什么用,只是为了最后一行不跟中文粘在一起.....另外,产品经理傻逼（这是惯例）
return 0;}
