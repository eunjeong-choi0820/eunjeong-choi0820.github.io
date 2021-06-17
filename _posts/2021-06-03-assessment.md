---
layout: single
title: "수행평가 정리" 
toc: true
toc_sticky: true
toc_label: 순서
catergories: 수업내용

---

### 01. 사주보기 

출생연도-월+일의 마지막 자리 숫자가 0이면 '대박' 아니면 '그럭저럭'
~~~c
#include <stdio.h>
int main(void){ 
  int year,month,day,result;
  
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
~~~


### 02. 3개의 터널 통과

지원이는 170cm인 차를 타고 3개의 터널을 통과한다. 3개의 터널 높이를 차례대로 입력하여 터널을 지나갈 수 있다면 '무사 통과'를출력하고 충돌이 일어난다면 '충돌'을 출력하고 가장 먼저 충돌하는 터널 높이도 출력하는 프로그램을 작성하라.
~~~c
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
  return 0;
}
~~~
---

### 03.이 달은 며칠까지 있을까?
 연도와 월을 알고 있을 때 그 달의 마지막 날을 구하는 프로그램을 작성하시오.
 ~~~c
 #include <stdio.h>
 main()
 {
 int a,b;
 printf("연도와 월을 입력하세요: ");
 scanf("%d%d", &a, &b);
 printf("%d년의 %d월의 마지막 날은", a,b);
 if(b==1 || b==3 || b==5 || b==7|| b==8 ||b==10 || b==12)
printf("31일");
else if(b==4 || b==6 || b==9 || b==11)
printf("30일");
else
{
if(a%4==0 && a%100!9 || a%400==0)
printf("29일");
else
printf("28일");
}
printf("입니다.\n");
}
~~~
 
