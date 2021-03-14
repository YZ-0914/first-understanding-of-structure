# first-understanding-of-structure
#define _CRT_SECURE_NO_WARNINGS 1
#include<stdio.h>

//描述一个学生
//名字 年龄 电话 性别
//struct  结构体关键字
//stu    结构体标签
//struct stu    结构体类型
//结构体声明是一条语句，后面要有分号
//struct stu
//{
//	//成员变量
//	char name[20];
//	short age;
//	char tele[12];
//	char sex[5];
//}s1,s2,s3;//三个全局结构体变量，尽量少用全局变量

//typedef struct stu
//{
//	//成员变量
//	char name[20];
//	short age;
//	char tele[12];
//	char sex[5];
//}stu;

//
//int main()
//{
//	stu s1;
//	struct stu s2;
//	return 0;
//}

//struct Point
//{
//	int x;
//	int y;
//}p1;//声明类型的同时定义变量p1
//struct Point p2;//定义结构体变量p2

//typedef struct stu
//{
//	//成员变量
//	char name[20];
//	short age;
//	char tele[12];
//	char sex[5];
//}stu;
//
//
//int main()
//{
//	stu s1 = {"张三",20,"13523453456","男"};//局部变量
//	struct stu s2={"旺财",30,"13223454567","保密"};
//
//	return 0;
//}

//struct S
//{
//	int a;
//	char c;
//	char arr[20];
//	double d;
//};
//struct T
//{
//	char ch[10];
//	struct S s;
//	char *pc;
//};
//
//int main()
//{
//	char arr[] = "hello\n";
//	struct T t = { "hehe", {100,'w',"hello world",3.14}, arr};
//	printf("%s\n", t.ch);//hehe
//	printf("%s\n", t.s.arr);//hello world
//	printf("%lf\n", t.s.d);//3.14
//	printf("%s\n", t.pc);//hello
//	return 0;
//}

//typedef struct stu
//{
//	//成员变量
//	char name[20];
//	short age;
//	char tele[12];
//	char sex[5];
//}stu;
//
//void Print1(stu s)
//{
//	printf("name:%s\n", s.name);
//	printf("age:%d\n", s.age);
//	printf("tele:%s\n", s.tele);
//	printf("sex:%s\n", s.sex);
//}
//
//void Print2(stu* ps)
//{
//	printf("name:%s\n", ps->name);
//	printf("age:%d\n", ps->age);
//	printf("tele:%s\n", ps->tele);
//	printf("sex:%s\n", ps->sex);
//}
//int main()
//{
//	stu s = {"李四",20,"13523453456","男"};//局部变量
//	//打印结构体数据
//	//Print1和Print2相比较Print2会更好
//	Print1(s);
//	Print2(&s);
//	return 0;
//}

int Add(int x, int y)
{
	int z = 0;
	z = x + y;
	return z;
}
int main()
{
	int a = 10;
	int b = 20;
	int ret = 0;
	ret = Add(a, b);
	return 0;
}
