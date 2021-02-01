# -
新手学习//实现两头缩进
#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>
#include<stdlib.h>
#include<string.h>
#include<windows.h>

int main()
{
	char arr1[] = "welcome to here!!!!";
	char arr2[] = "                   ";
	int left = 0;
	int right = strlen(arr1) - 1;
	while (left <= right)
	{
		arr2[left] = arr1[left];
		arr2[right] = arr1[right];
		printf("%s\n", arr2);
		Sleep(500);//停留0.5s
		system("cls");
		left++;
		right--;
	}
	system("pause");
	return 0;
}
