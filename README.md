# 2021-04-21
再次学习结构体！并观看进阶课程。

进阶课程第一周编程作业：
#include<stdio.h>

int main(int argc,char const *argv[])
{
	int r[200];
	int a,b;
	printf("Please input a/b(10<=a<b<100):");
	scanf("%d/%d",&a,&b);
	
	int i;
	int flag = 1;
	printf("0.");
	for (i=0; i<200&&flag ; i++)
	{
		r[i] = a * 10 / b;
		printf("%d",r[i]);
		a = a * 10 % b;
		if (a == 0)
			flag = 0;
	}
	printf("\n");
	return 0; 
}
