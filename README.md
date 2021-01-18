题目：一球从100米高度自由落下，每次落地后反跳回原高度的一半；再落下，求它在第10次落地时，共经过多少米？第10次反弹多高？
#include<stdio.h>
int main()
{
    float s,h;
    h=100,s=100;
    h=h/2;
    for(int i=1;i<10;i++)
    {
       s+=h*2;
       h=h/2;
    }
    printf("第10次落地时，共经过%f米，反弹高度%f米\n",s,h);
    return 0;
}
