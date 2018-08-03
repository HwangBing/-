#include<stdio.h>
int main(){
	int a,b,c=0;
	printf("请输入一个正三位数:");
	scanf("%d",&a);
	if(99<a&&a<10000){
		while(a>0){
			b=a%10;
			if(b>0){
				c=c*10+b;
			}
			a/=10;
		}
		printf("%d",c); 
	
	} else{
		printf("输入有误"); 
	}
} 
