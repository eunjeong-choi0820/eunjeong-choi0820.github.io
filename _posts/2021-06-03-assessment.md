---
layout: single
title: "수행평가 정리" 
toc: true
toc_sticky: true
toc_label: 순서

### 01. 사주보기 

#include <stdio.h>
int main(void)
{ int year,month,day,result;
printf("당신의 사주를 봐드립니다.\n");
printf("연도 월 일을 차례대로 입력하세요 : ");
scanf("%d,%d,%d",&year,&month,&day);
result=(year-month+day)%10;
if(result==0)
printf("당신의 사주는 대박입니다.\n");
else
printf("당신의 사주는 그럭저럭입니다.\n");
return 0;
}
---

### 02. 3개의 터널 통과
지원이는 170cm인 차를 타고 3개의 터널을 통과한다. 3개의 터널 높이를 차례대로 입력하여 터널을 지나갈 수 있다면 '무사 통과'를출력하고 충돌이 일어난다면 '충돌'을 출력하고 가장 먼저 충돌하는 터널 높이도 출력하는 프로그램을 작성하라.
#include<stdio.h>
int main()
{
int a,b,c;
printf("터널의 높이를 차례대로 입력하세요: ");
scanf("%d%d%d", &a,&b,&c);
if(a<=170)
printf("충돌 %d", a);
else if (b<=170)
printf("충돌 %d" ,b);
else if (c<=170)
printf("충돌 %d" ,c);
else
printf("무사통과");
}

