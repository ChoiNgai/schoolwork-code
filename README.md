# schoolwork-code
＃This C++ program was written at school time.——ChoiNgai
#include "stdafx.h"
#include "iostream"
using namespace std;

int main( )
{
	//int *p;
	int i,j;
	int a[3][4];
	int b[4][3];
	int p[4][4];

	for(i=0;i<3;i++){

		for(j=0;j<4;j++){
			
			cin>>a[i][j];
			};
	};

	for(i=0;i<4;i++){
	
	for(j=0;j<3;j++){
			
			cin>>b[i][j];
		};
	};
	
	int k;

	for (i=0;i<4;i++){	//第i行

	for(j=0;j<4;j++){			//第j列

		*(*(p+i)+j)=0;
		for(k=0;k<3;++k){
			*p[k]=b[i][k]*a[k][j];

			*(*(p+i)+j)=*(*(p+i)+j)+*p[k];
		};
		cout<<*(*(p+i)+j)<<"  ";
	};
	cout<<endl;
	};

	return 0;
}
